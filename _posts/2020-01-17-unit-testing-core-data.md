---
title: "A note on iOS unit testing with Core Data"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - in the trenches
  - quick tips
  - programming
  - iOS
  - Core Data
  - unit testing
---

**Here's a good one** that held me up for almost a day.  I was trying to integrate Core Data testing into a unit testing suite.  

All was going well.  We were using a database (really an object store to be pedantic) to be loaded and stored by the app, but to test the storage manager the usual best practice is to mock up a purely in-memory database and exercise that.

Only problem was, the tests wouldn't work, and after a few hours of research I still couldn't figure out why.  It seemed like the issue was so basic that there was no way that I had discovered a bug in the system itself, so most likely (99.99%) I had done something wrong. Yet the issue seemed to come out of nowhere that I could access, and rebuilding the very simple project from scratch had no effect.

<!--more-->

It had two parts —

The app would build and run normally with no errors. But in the testing phase the console would include (chunked for ease of understanding):

```
objc[16266]: Class FooItem is implemented in both 
/Users/xxx/Library/Developer/CoreSimulator/Devices/###/data/Containers/Bundle/Application/###/MyApp.app/MyApp (0x1087577a0) 
and 
/Users/xxx/Library/Developer/Xcode/DerivedData/Build/Products/Debug-iphonesimulator/MyApp.app/PlugIns/MyAppTests.xctest/MyAppTests (0x108d68d40). 
One of the two will be used. Which one is undefined.
```

Then each test would hang, whereupon the console would emit:
```
Could not cast value of type 'MyApp.FooItem' (0x600003fc1ab0) to 'MyAppTests.FooItem' (0x108d68d40).
```

Now, `FooItem` was being defined in the Core Data data model file. And searching within the project turned up an automatically-generated file of pure boilerplate that warned that it shouldn't be edited. Manually generating the file yielded only extra errors about duplicate files. Prowling through build settings to see if something was being copied when it shouldn't brought no joy either.

Doing web searches on elements of the error descriptions led to complaints about frameworks being mishandled.  But I wasn't adding any frameworks!

By this time I was willing to go to lower-bandwidth sources, like video. 

Video may require far more bandwidth to transmit and perceive, but when considered in this context — the communication of organized technical information to another human — I can basically get about five times as much information/second from text (or even better, text with illustrative images) than from video. In addition, text can be skimmed or accessed randomly (to locate just that much-needed nugget of info), and leaves out all the "um"s and "uh"s and other hesitations that non-professional speakers tend to have. Video is brilliant at setting a scene in a quarter of a second when applied to animal and fail videos, less so when presenting code and concepts.
{: .notice}

