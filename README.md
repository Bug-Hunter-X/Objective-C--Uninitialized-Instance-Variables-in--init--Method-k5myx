# Objective-C: Uninitialized Instance Variables in `init` Method

This repository demonstrates a common error in Objective-C: accessing uninitialized instance variables within a class's `init` method.  This can lead to unexpected behavior or crashes.

The `bug.m` file shows the incorrect implementation, while `bugSolution.m` provides the corrected version.  The issue arises from accessing instance variables before they've been fully initialized after `self = [super init];` check.  Always ensure all instance variables are properly initialized before using them within the initializer to avoid such problems. 