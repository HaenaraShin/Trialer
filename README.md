# Trialer

[![](https://jitpack.io/v/pzienowicz/Trialer.svg)](https://jitpack.io/#pzienowicz/Trialer)
[![API](https://img.shields.io/badge/API-14%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=14) 
![GitHub issues](https://img.shields.io/github/issues/pzienowicz/Trialer.svg?style=flat-square)
[![Build Status](https://travis-ci.org/pzienowicz/Trialer.svg?branch=master)](https://travis-ci.org/pzienowicz/Trialer)  


A small and simple library for managing trial period in your android app.

Installation
------------

### Gradle
Add this to your root build.gradle file under repositories:
```
allprojects {
	repositories {
		maven { url "https://jitpack.io" }
	}
}
```
Add this to your app level build.gradle as dependency:

    com.github.pzienowicz:Trialer:1.0.0

### Maven
```
```

## Usage

### Kotlin
```java
Trialer().apply {
    buildDate = BuildConfig.BUILD_TIME,
    daysAfterBuild = 30
    trialEndedListener = object: TrialEndedListener {
    	override fun onTrialEnded() {
		
        }
    }
}.valid()
```


### Java
```java

```

