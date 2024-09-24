---
layout: post
title: TwinCAT 3 | Using Source Control in TwinCAT (Git) | Introduction
date: 2024-09-20 14:38 -0300
categories: [TwinCAT 3 PLC, 1. Using Source Control in TwinCAT (Git)]
tags: [TwinCAT 3, Git, Source Control]
---

> Remember that this page isn't affiliated with BECKHOFF and **MUST NOT** be used as a official documentation. For that, please refer to the official BECKHOFF webpage.
{: .prompt-danger }

> All my content is free and the main goal is to provide TUTORIALS. If you plan to use ANY of it in production or application, it **MUST** be thoroughly tested before implemented (use the code at your own risk).
{: .prompt-danger }

# Introduction

In today's world, Automation and Machinery Technology (AT) are increasingly merging with Information Technology (IT). It's no surprise that the shortcuts and powerful tools from **traditional IT programming**, such as Data Analysis Tools and Dev/DevOps tools, are gradually making their way into the Automation Technology realm.

One of the most challenging tasks in the programming world, since its inception, has been **storing and tracking** changes in application code. Unlike our IT counterparts, in AT, one common solution is to start a project with a folder name or a large `.zip` file like this:

- Machine_That_Does_Something_20220901_v0  
- Machine_That_Does_Something_20220901_v0.zip

Once you have a stable version, you update the folder name:

- Machine_That_Does_Something_20220901_v1_stable  
- Machine_That_Does_Something_20220901_v1_stable.zip

After repeating this process several times, you'll end up with an unwieldy list of long folder names, containing little information about the actual changes made inside:

- Machine_That_Does_Something_20220901_v0  
- Machine_That_Does_Something_20220901_v1_stable  
- Machine_That_Does_Something_20220901_v1.1_maybe_stable  
- Machine_That_Does_Something_20220901_v2.12_is_it_stable  
- Machine_That_Does_Something_20220901_v3.0_pray_this_is_stable_with_1.101_changes

Given these files, how do we answer three basic questions?  
1. What did my customer request or what changes did I make between version v0 and v1?  
2. Why is version 2.12 with the required changes less stable than version 1.1?  
3. In case of multiple programmers, who made the changes between version v0 and v1?

Lastly, but critically, something we’re not used to in the Automation Industry is **Code Review!** 

1. How can we establish an effective code review process if my company is using folder names for source control?

With these basic questions, we can demonstrate that using folder names for source control isn’t the best solution.

Perhaps it's the same motivation that led Linus Benedict Torvalds (a.k.a. the creator of Linux) to develop one of the most remarkable source control tools, named **Git**.

If you don't know what is Git, I really recommend Programming with Mosh video that explains it!

<iframe width="560" height="315" src="https://www.youtube.com/embed/2ReR1YJrNOM?si=EMQ82qnezZUxvRXL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

It would be fantastic if we could utilize this powerful tool, which is extensively tested and widely used in IT for source control. However, unfortunately, as our colleague Jakob Sagatowski points out,

>The automation industry is really underdeveloped regarding version control. Most PLC vendors use their own proprietary way to store source code, which results in that the PLC vendors and third party suppliers charge you big money for something so basic as version control, making the barrier for people not doing version control even higher. 

>The vendors are either providing their own proprietary version control system and the tools that only works with their particular brand, or there are vendors that build a system on top of the popular version control systems but then it only works if you use their software to do the version control. Not only are these tools expensive, but they are also add complexity and additional dependencies for external software. 

Despite what is common in the automation industry, Beckhoff provides us with the integration of Git directly merged into the TwinCAT 3 XAE Shell, and they do not charge a single cent for this, and you can not only use the TwinCAT 3 XAE Shell Git Interface, but any Git Interface to work with TwinCAT 3 PLC code, like TortoiseGit, GitBash or GitHub Desktop.

I recommend you continue your reading following one of these options below, based on which interface you want to work it:

## Using TwinCAT 3 Shell Git Interface - **Team Explorer** | My own content
[Link to my page content.]({% link _posts/2024-09-24-twincat-3-using-source-control-basics.md %})

## Using a mix of TortoiseGit and TwinCAT 3 Shell Git Interface - **Team Explorer** | Jakob Sagatoski
[Jakob Sagatowski Tutorial | English](https://youtu.be/1g6eYnlzKtA?si=Xhk_yBzREBt3z2vj)
<iframe width="560" height="315" src="https://www.youtube.com/embed/1g6eYnlzKtA?si=Xhk_yBzREBt3z2vj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Using GitHub Desktop | Automacaoweb
[Post about source control - Automacaoweb | Portuguese](https://automacaoweb.wordpress.com/2022/07/25/tc3-controle-de-versao/)
