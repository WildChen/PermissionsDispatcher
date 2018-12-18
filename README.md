# PermissionsDispatcher [![Build Status](https://travis-ci.org/permissions-dispatcher/PermissionsDispatcher.svg?branch=master)](https://travis-ci.org/permissions-dispatcher/PermissionsDispatcher)

- [**Kotlin support**](https://github.com/hotchemi/PermissionsDispatcher/blob/master/doc/kotlin_support.md)
- [**Special Permissions support**](https://github.com/hotchemi/PermissionsDispatcher/blob/master/doc/special_permissions.md)
- **100% reflection-free**

PermissionsDispatcher provides a simple annotation-based API to handle runtime permissions.

This library lifts the burden that comes with writing a bunch of check statements whether a permission has been granted or not from you, in order to keep your code clean and safe.

For more information please see [the website](https://permissions-dispatcher.github.io/).

## Download

NOTE: 4.x only supports [Jetpack](https://developer.android.com/jetpack/). If you still use appcompat 3.x is the way to go.

To add PermissionsDispatcher to your project, include the following in your **app module** `build.gradle` file:

`${latest.version}` is [![Download](https://api.bintray.com/packages/hotchemi/maven/permissionsdispatcher/images/download.svg)](https://bintray.com/hotchemi/maven/permissionsdispatcher/_latestVersion)

```groovy
dependencies {
  implementation "com.github.hotchemi:permissionsdispatcher:${latest.version}"
  annotationProcessor "com.github.hotchemi:permissionsdispatcher-processor:${latest.version}"
}
```

With Kotlin:

```groovy
apply plugin: 'kotlin-kapt'

dependencies {
  implementation "com.github.hotchemi:permissionsdispatcher:${latest.version}"
  kapt "com.github.hotchemi:permissionsdispatcher-processor:${latest.version}"
}
```

Snapshots of the development version are available in [JFrog's snapshots repository](https://oss.jfrog.org/oss-snapshot-local/). 
Add the repo below to download `SNAPSHOT` releases.

```groovy
repositories {
  jcenter()
  maven { url 'http://oss.jfrog.org/artifactory/oss-snapshot-local/' }
}
```

## Licence

```
Copyright 2016 Shintaro Katafuchi, Marcel Schnelle, Yoshinori Isogai

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
