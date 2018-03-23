# ViewUsage
## 用于总结一些View的方便用法

### 1、一个带有图标和文字的控件

![](https://github.com/Ruijiao/ViewUsage/blob/master/resouce/i_loading.png)

用一个TextView即可搞定

    <TextView
          android:layout_width=""wrap_content""
          android:layout_height=""63dip""
          android:layout_centerHorizontal=""true""
          android:layout_gravity=""center""
          android:drawablePadding=""1dp""
          android:drawableTop=""@drawable/i_comimit""
          android:gravity=""center_horizontal""
          android:paddingBottom=""3dp""
          android:paddingTop=""3dp""
          android:text=""发布""
          android:textColor=""@color/txt_normal""
          android:textSize=""11dip"" />

### 2、一个旋转图标，例如加载中的提示git图

![](https://github.com/Ruijiao/ViewUsage/blob/master/resouce/g_loading.gif)

 可以用 ProgressBar 控件

         <ProgressBar
            android:layout_width="80dp"
            android:layout_height="80dp"
            android:layout_marginTop="0dp"
            android:id="@+id/progress1"
            android:indeterminateDrawable="@drawable/progress_gear_fu"
            android:layout_alignParentTop="true"
            android:layout_centerHorizontal="true" />

我们看看progress_gear_fu文件怎么写的

    <?xml version="1.0" encoding="utf-8"?>   
    <rotate xmlns:android="http://schemas.android.com/apk/res/android"  
        android:drawable="@drawable/i_loading"
        android:pivotX="50%"  
        android:pivotY="50%"  
        android:fromDegrees="0"  
        android:toDegrees="720" />


