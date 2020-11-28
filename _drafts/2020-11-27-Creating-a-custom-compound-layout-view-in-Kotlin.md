---
layout: post
title: Creating a custom compound layout view in Kotlin
subtitle: We've created a custom layout dozens of times in Java, but how does it work in Kotlin
tags: [Kotlin, Android, UI]
comments: true
---

The single-responsibility principle is core concept of the [SOLID](https://en.wikipedia.org/wiki/SOLID) principles of writing good code. This can also be applied to UI components. We can pull all of the components needed into it's own isolated component and supply it with the data needed to display. This becomes especially useful when adding a custom set of views in a Recycler view when we can just hand the ViewHolder a specific view component, it's entity, and not have to fumble around with all the subviews ids in every RecyclerView we use it in. But, enough talk, let's get into it.

First, you want to create a Kotlin class representing the view.
