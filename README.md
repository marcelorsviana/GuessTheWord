ViewModel and ViewModelFactory - Starter Code
==================================

Use as starter code for the ViewModel codelab.

Introduction
------------

This starter app is a two player game, GuessTheWord. It is a word guessing app you can play with one or more friends. To play, hold the device in landscape, facing away from you with your thumbs on the **Skip** and **Got It** buttons. Your friends can then give you clues to help you guess the word. If you get the word right, press **Got It**. If you're stuck, press **Skip**.
You will modify the app to use Architecture components and best practices.

Pre-requisites
--------------

You need to know:
- How to open, build, and run Android apps with Android Studio.
- How to use the Navigation Architecture Component
- Passing the data between navigation destinations.
- Read the logs using the Logcat.


Getting Started
---------------

1. Download and run the app.

License
-------

Copyright 2019 Google, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.

# GuessTheWord
## Android Kotlin Bootcamp from Google Developer website
### CODELAB: Android Kotlin Fundamentals:5.1 ViewModel - https://developer.android.com/codelabs/kotlin-android-training-view-model?index=..%2F..android-kotlin-fundamentals#0


#### **What I learned:**</br>
- How to use the recommended Android app architecture.
- How to use the Lifecycle, ViewModel, and ViewModelFactory classes in the app.
- How to retain UI data through device-configuration changes.
- What the factory method design pattern is and how to use it.
- How to create a ViewModel object using the interface ViewModelProvider.Factory.

#### **What I did:**</br>
- Add a ViewModel to the app, to save app's data so the data survives configuration changes.
- Use ViewModelFactory and the factory-method design pattern to instantiate a ViewModel object with constructor parameters.


------------------------------------------------------------

### CODELAB: Android Kotlin Fundamentals: LiveData and LiveData observers - https://developer.android.com/codelabs/kotlin-android-training-live-data#0

#### **What I learned:**</br>
- What makes LiveData objects useful.
- How to add LiveData to the data stored in a ViewModel.
- When and how to use MutableLiveData.
- How to add observer methods to observe changes in the LiveData.
- How to encapsulate LiveData using a backing property.
- How to communicate between a UI controller and its corresponding ViewModel.

#### **What I did:**</br>
- Use LiveData for the word and the score in the GuessTheWord app.
- Add observers that notice when the word or the score changes.
- Update the text views that display changed values.
- Use the LiveData observer pattern to add a game-finished event.
- Implement the Play Again button.


------------------------------------------------------------

### CODELAB: Android Kotlin Fundamentals: Data binding with ViewModel and LiveData - https://developer.android.com/codelabs/kotlin-android-training-live-data-data-binding#0

#### **What I learned:**</br>

- How to use elements of the Data Binding Library.
- How to integrate ViewModel with data binding.
- How to integrate LiveData with data binding.
- How to use listener bindings to replace the click listeners in a fragment.
- How to add string formatting to data-binding expressions.

#### **What I did:**</br>

- The views in the GuessTheWord layouts communicate indirectly with ViewModel objects, using UI controllers (fragments) to relay information. In this codelab, I bound the app's views to ViewModel objects so that the views communicate directly with the ViewModel objects.
- I changed the app to use LiveData as the data-binding source. After this change, the LiveData objects notify the UI about changes in the data, and the LiveData observer methods are no longer needed.

------------------------------------------------------------

### CODELAB: Android Kotlin Fundamentals:5.4 LiveData transformations - https://developer.android.com/codelabs/kotlin-android-training-live-data-transformations#0

#### **What I learned:**</br>

- How to use Transformations with LiveData

#### **What I did:**</br>

- Add a timer to end the game.
- Use Transformations.map() to transform one LiveData into another.
