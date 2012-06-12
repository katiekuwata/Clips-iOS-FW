Clips-iOS-FW
============

This project is based on the project clipsmm-mobile for MAC OS X. I could not convert the project to a framework project for iOS so I created this framework project from scratch. 

Steps created this project
--------------------------
* Downloaded the file (CLIPS_6.30_Beta_Mac_OS_X_Installer_R1.pkg) from 
http://sourceforge.net/projects/clipsrules/files/CLIPS/6.30/ 

* Unzip "Source Code.zip" file

* I created universal framework similar steps described in 
[Building a Universal Framework for iOS](http://spin.atomicobject.com/2011/12/13/building-a-universal-framework-for-ios/)

Universal Framework
-------------------
* Comment from above link describe the universal framework well:
A universal framework can be defined as a framework that contains a binary which has been built for a number of architectures (armv6, armv7, i386) and can be statically1 linked against. This is particularly useful in iOS development because an application can be built for the simulator (i386) and the device (armv6, armv7). In fact, I need this for ZeroMQ project.

* Universal framework include arm6 and arm7 binary as well as i386 so we need to remove i386 for the production deployment.

TODO
----

* TestFWCalc is a sort of wrapper I am planning to create wrapper interface for the CLIPS engine. Explorer if we can use clipsmm wrapper.

Discussion
----------
[iOS Porting Thread](https://groups.google.com/d/topic/CLIPSESG/Birk6kK8opk/discussion)
