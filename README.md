Material Loading Indicator
=============

<img src="https://i.imgur.com/dzQyBAj.gif" height="400">

Description
------------
A simple implementation of [Material Progress Indicators](https://material.io/components/progress-indicators). This library allows the showing of progress indicators anywhere in the app programmatically. 

## Gradle Dependency

 ``` gradle
dependencies {
    implementation 'com.github.gemeauxph:MaterialLoadingIndicator:1.0.0'
 }
 ```

## Setup

 ``` 
 buildscript {
    repositories {
     .......
        maven { url 'https://jitpack.io' }
    }
}

allprojects {
    repositories {
     .......
        maven { url 'https://www.jitpack.io' }
    }
}
 ```

## Sample Usage
- Kotlin
```
val progressIndicator = MaterialCircularIndicator(this)
```
           
- Java
```
MaterialCircularIndicator progressIndicator = new MaterialCircularIndicator(this);
```

```
progressIndicator.setCanceleable(true)
progressIndicator.setIndicatorSize(100) //In DP
progressIndicator.setTrackThickness(10) //In DP
progressIndicator.setTrackCornerRadius(10) //In DP
progressIndicator.setIndicatorColor(Color.parseColor("#4287F5"))
progressIndicator.setTrackColor(Color.parseColor("#AEC9F5"))
progressIndicator.setMessageTextColor(Color.parseColor("#000000"))
progressIndicator.setLoadingMessage("Loading...")
progressIndicator.setTextSize(20f) //Float value
progressIndicator.setMessageTypeFace(Typeface.BOLD)
progressIndicator.setProgress(90) //1 to 100
progressIndicator.setIndeterminate(true)
progressIndicator.setBackgroundColor(Color.parseColor("#FFFFFF"))
```

## Customizations

Method | Default Value
------------            |   -------------
setCanceleable()        |   false
setIndicatorSize()      |   64
setTrackThickness()     |   7
setTrackCornerRadius()  |   0
setIndicatorColor()     |   #4287F5
setTrackColor()         |   #AEC9F5
setMessageTextColor()   |   
setLoadingMessage()     |
setTextSize()           |
setMessageTypeFace()    |   Typeface.NORMAL
setProgress()           |
setIndeterminate()      |   true
setBackgroundColor()    |   Transparent

