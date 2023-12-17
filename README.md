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
MIT License

Copyright (c) 2023 Samyak Kamble

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
