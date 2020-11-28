---
layout: post
title: Enable Data Binding
subtitle: Kotlin Synthetics are being phased out, here's how you enable DataBinding
tags: [Kotlin, Android, UI]
comments: true
---

## Enable Android DataBinding in Android Studio 4.1.1

Open your module's `build.gradle` and add the following code:

First make sure you are using Kotlin Annotation Processing and have that added in your project.

At the top of your `build.gradle`, you'll see `plugins`. Add

```
  id 'kotlin-kapt'
```

to the bottom.

Next, we're actually going to enable DataBinding.

```
android {
  buildFeatures {
    dataBinding true
  }
}
```

And that's it. You should be able to add `layout` tags to your xml files, and use `DataBindingUtil` in your classes where you need it.

If you need to make a custom view using DataBinding, [check out my post](https://antlip.dev/2020-11-27-Kotlin-Custom-View-with-DataBinding/).

Happy Coding.
