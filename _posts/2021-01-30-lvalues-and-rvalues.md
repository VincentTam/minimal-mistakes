---
layout: blog-single
classes: wide
title:  "Lvalues and Rvalues in C++"
excerpt: "Understanding the meaning of lvalues and rvalues in C++"
date: 2021-01-30
last_modified_at: 2021-01-31
permalink: /blog/2021/01/30/lvalues-and-rvalues/
tags:
  - c++
---

In this blog post, we will try to understand the meaning behind the C++ concepts: **lvalues** and **rvalues**. We, C++ Developers, use to write a lot of C++ codes and already familiar with these concepts however, since these are formal definitions, we don't even notice that we are using these in our day-to-day coding life. Now, let's try to understand these concepts in informal way.
{: .text-justify}

Consider the following example:

```c++
int x = 100;
```
