---
layout: essay
type: essay
title: Reflect On Configuration Management
date: 2017-01-30
labels:
  - ICS 314
  - Configuration Management
---

Configuration management is tracking the changes made to the files that make up a system. When good configuration management techniques are employed, it is easy to revert to a functioning version of the system should something stop working as intended after an update. Tracking the changes also means having a relatively easy way to find what caused the problem.

Proper configuration management is important. More so when working with a team, which in the workplace is bound to happen. When working with a team it is difficult to know what everyone is has changed, there needs to be an efficient way to track the changes so that if something fails to work properly the cause of the problem can be found regardless of how many members of the team are available at the time when the problem was found.

Although I have yet to fall victim to poor configuration management I am aware of what can happen. A friend of mine had been working on a group assignment, he just added some new code and went to test it. It went horribly wrong with the program endlessly generating an empty file. After killing the process he went to inspect his code to see what he did wrong. After a day of finding nothing that would cause the problem in his own code he realized that another member had changed something in a completely separate part of the code, which happened to be the source of the problem. Had they used proper configuration management techniques it would have taken less time to inspect the  changes that had been made between the time the program was functioning and when he had tested it, thus saving his time and the assignment would have progressed faster.

### Git and GitHub

I think that GitHub is popular because of Git. Git allows the user to work offline, therefore as long as the user has access to the computer their copy of the repository is saved on they can continue to work and prepare updates. Then when the user gains internet access the changes can be pushed to the main repository. Git also makes it easy to create new braches of a repository and a developer could take the project in different direction than the original. Without Git, GitHub would be like any other website that provides source code hosting services and there would be no change in how configuration management is done.