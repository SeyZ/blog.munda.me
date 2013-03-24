title: Continuous Development, a part of the Continuous Integration concept ?
author: Sandro Munda
date: 2013-03-24 22:10
tags: continuous-integration, software, python, tool

Continuous Integration, I know what it is!
==========================================

Developers, you all know what Continuous Integration is. For example, say that you begin a new feature. You write some code, some unit tests, etc. Once done, you push your changes to your remote SCM repository (e.g. git). Your continuous integration then tool detects the changes and runs some integration tasks, e.g. unit tests, packaging, deployment, etc. At this stage, a report is available and you can check if something went wrong.

Are you really sure to cover all the integration process?
=========================================================

But wait, how can you be sure that your feature is "mergeable" in your main branch ? You could do it at the end of the process described above... but it's late! Wouldn't you prefer to detect possible merge problems as soon as possible ? This helps to avoid merge conflicts and therefore, merge hells.

Introducing a new kind of tool: Baboon
======================================

That's why I created Baboon, a free Python tool to detect merge conflicts in realtime. Each time a file is saved, Baboon checks if there is any problem. If so, the whole team is warned. It's now time to blame the culprit! The detected conflict is super easy to solve, because it's small. Remember: you are notified in realtime!

Your code is now continuously integrated from the development to the deployment.

Information
===========

http://baboon-project.org

The source code is available on Github http://github.com/SeyZ/baboon under the MIT license.

Thanks for feedbacks, suggestions, etc.
