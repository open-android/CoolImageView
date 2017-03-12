
项目地址：<https://github.com/open-android/CoolImageView>

# 一分钟实现QQ首页动画特效

# Preview
![CoolImageView](myapplication/gif/CoolImageView.gif)

![coolImag](myapplication/gif/coolImag.gif)

### 欢迎关注微信公众号、长期为您推荐优秀博文、开源项目、视频

![](http://oi5nqn6ce.bkt.clouddn.com/itheima/booster/code/qrcode.png)


## 使用步骤

### 1. 在project的build.gradle添加如下代码(如下图)

	allprojects {
	    repositories {
	        maven { url "https://jitpack.io" }
	    }
	}

![](http://upload-images.jianshu.io/upload_images/4037105-2faa5daca3bfe8a0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
	

	
### 2. 在Module的build.gradle添加依赖

    compile 'com.github.open-android:CoolImageView:0.1.0'
    

### 3.布局文件中使用

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/activity_main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    >
    
    <com.itheima.imageview.CoolImageView
        android:layout_width="wrap_content"
        android:layout_height="300dp"
        android:src="@mipmap/qq"
        app:direction="horizontal"

       >
    </com.itheima.imageview.CoolImageView>

    <com.itheima.imageview.CoolImageView
        android:layout_marginTop="@dimen/activity_vertical_margin"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:src="@mipmap/qq_"
        app:direction="vertical"
        >
    </com.itheima.imageview.CoolImageView>
</LinearLayout>


```

