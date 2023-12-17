[![](https://jitpack.io/v/OmaPrakash/CircleImageView.svg)](https://jitpack.io/#OmaPrakash/CircleImageView)
![GitHub](https://img.shields.io/github/license/OmaPrakash/CircleImageView)

<p align="center">
  <h1 align="center">CircleImageView</h1>
</p>

- ⚡  If You want to join us than message on <a href="arrowwouldpro@gmail.com">Mail</a>
 

> Note: `-- Apache License 2.0` you can't Publish any Source code without permission.

# 

<p align="center">If you like my work and Source Code is really helpful for you, <strong>Show Some Love</strong></p>

<p align="center">
    <a >
     <img src=""/>
    </a>
  </p>

It uses a BitmapShader and does not:

- create a copy of the original bitmap
- use a clipPath (which is neither hardware accelerated nor anti-aliased)
- use setXfermode to clip the bitmap (which means drawing twice to the canvas)

As this is just a custom ImageView and not a custom Drawable or a combination of both, it can be used with all kinds of drawables, i.e. a PicassoDrawable from Picasso or other non-standard drawables (needs some testing though).



## How to:
- gradle

Add the JitPack repository to your build file.
Add this in your root `settings.gradle` file (**not** your module `build.gradle` file):

```gradle

dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.PREFER_SETTINGS)
    repositories {
    ....
        maven { url "https://jitpack.io" }
        ...
    }
}
```

Then, add the library to your module `build.gradle`

```gradle
dependencies {
  implementation 'com.github.samyak2403:CircleImageView:(letest Release)'
}
```


```xml
<com.samyak2403.CircleImageView
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/profile_image"
    android:layout_width="96dp"
    android:layout_height="96dp"
    android:src="@drawable/profile"
    app:civ_border_width="2dp"
    app:civ_border_color="#FF000000"/>
```
- maven

```
<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
</repositories>

```

```
<dependency>
	    <groupId>com.github.samyak2403</groupId>
	    <artifactId>CircleImageView</artifactId>
	    <version>Tag</version>
</dependency>
```



### License
```
  Copyright 2023 samyak

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
