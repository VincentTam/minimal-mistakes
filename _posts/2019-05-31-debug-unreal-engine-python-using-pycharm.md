---
title: "Debug Unreal Engine Python using PyCharm"
categories:
  - Programming
tags:
  - Python
  - Unreal Engine 4
comments: true
---
{: .text-justify}
If you are using [Unreal Engine Python](https://github.com/20tab/UnrealEnginePython) you *might* want to debug your program without putting ```print()``` everywhere.
Here is what I use to debug Unreal Engine python code from PyCharm.

1. Configure your python interpreter

   Add a new python interpreter : [https://www.jetbrains.com/help/pycharm/configuring-python-interpreter.html#add_new_project_interpreter](https://www.jetbrains.com/help/pycharm/configuring-python-interpreter.html#add_new_project_interpreter)

   If you use the embedded python interpreted, it should be located here ```Engine\Plugins\UnrealEnginePython\Binaries\Win64\python.exe```

2. Create a remote debug configuration

   On the run/debug configuration selector, select ```Edit Configurations...```

   ![edit config](/assets/images/articles/debug-unreal-engine-python-using-pycharm/addconfiguration.png){: .align-center}

   Create a new configuration by clicking the ```+``` button and ```Python Remote Debug```.

   ![add remote](/assets/images/articles/debug-unreal-engine-python-using-pycharm/addremoteconfig.png){: .align-center}

   Setup your configuration by giving it a name, choose a port (for example ```60058```), check ```Redirect output to console``` and uncheck ```Suspend after connect```. Then, click ```OK```.

   ![setup remote](/assets/images/articles/debug-unreal-engine-python-using-pycharm/setupconfig.png){: .align-center}

3. Launch the debug configuration in PyCharm

   Select your debug configuration on the Run/Debug configuration selector on the top right of the window.

   ![enable remote](/assets/images/articles/debug-unreal-engine-python-using-pycharm/enableremote.png){: .align-center}

   Click the bug icon to launch the remote debugging ![bug](/assets/images/articles/debug-unreal-engine-python-using-pycharm/bug.png). It will wait for a remote connection.

   ![wait](/assets/images/articles/debug-unreal-engine-python-using-pycharm/wait.png){: .align-center}

4. Attach to the debugger in Unreal

   {: .text-justify}
   Execute the following code from the Unreal Engine Python editor.

   You'll have to change the ```pydev_path``` variable and use your own ```pydev``` directory from your PyCharm installation. 
   {: .notice--info}
   ```python
   import sys

   def attach_to_debugger(host, port):
       try:
           # TODO : Use your PyCharm install directory.
           pydev_path = "D:/PyCharm/PyCharm 2018.3.4/helpers/pydev"

           if not pydev_path in sys.path:
               sys.path.append(pydev_path)
           import pydevd
           pydevd.stoptrace()
           pydevd.settrace(
               port=port,
               host=host,
               stdoutToServer=True,
               stderrToServer=True,
               overwrite_prev_trace=True,
               suspend=False,
               trace_only_current_thread=False,
               patch_multiprocessing=False,
           )
           print("PyCharm Remote Debug enabled on %s:%s." % (host,port))
       except:
           import traceback
           traceback.print_exc()

   attach_to_debugger('localhost', 60058)
   ```

   {: .text-justify}
   If you don't want to execute this code every time you need to debug you application, you can call it from the [```ue_site.py```](https://github.com/20tab/UnrealEnginePython#the-ue_sitepy-file) file, but watch out, ```pydevd.settrace()``` will freeze the engine until you launch your remote debug configuration from PyCharm.

5. That should be it !

   Put some breakpoints in PyCharm and they should break when the code is executed.

   Sadly, despite having access to the content of your standard variables (list, dict...), you won't be able to get the content of ```unreal_engine.UObject``` and other Unreal related objects.

___

{: .text-justify}
If you are using VSCode, take a look at the [Remote Debugging documentation](https://code.visualstudio.com/docs/python/debugging#_remote-debugging) of the Python extension.
Unfortunately, the last time I tried it, I couldn't manage to hit the breakpoints since they were *Unverified* (greyed out).
