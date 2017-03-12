

# Preview
![CoolImageView](myapplication/gif/CoolImageView.gif)

step2:Add the following code to the root view of your layout:  
-----
```xml
xmlns:app="http://schemas.android.com/apk/res-auto"
```

step3:Add the widget code in the appropriate place in your xml file, Here's a sample implementation:  
-----
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

