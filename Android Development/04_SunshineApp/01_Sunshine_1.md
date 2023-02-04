### Sunshine App
1. There are 4 types of components that make up apps.
	1. Activity
	2. Service
	3. Content Provider
	4. Broadcast Receiver
---
#### Activity
1. Single focused thing that the user can do.
2. Responsible for creating the window that your application uses to draw and receive events from the system.
3. The OnCreate function inside the activity, contains setContent View, that causes XML Layout resource to be inflated converting everything in the XML file to hierarchy of view objects in memory.
4. Frame, Constraint and Linear Layout are three of the most common layouts.
5. Frame Layout is great for simple layouts where we only have one child view, which fills the entire content area.
6. If you had multiple items in it, they'd overlap.

---

#### Messaging Logging Display Levels
1. What a Terrible Failure (WTF)
2. Error
3. Warn
4. Info
5. Debug
6. Verbose