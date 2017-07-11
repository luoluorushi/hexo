---
title: android ui
date: 2017-06-26 10:35:01
tags:
---
### Window

1. 设置对话框等宽，位于屏幕底部
```java
Window window = getWindow();
WindowManager.LayoutParams params = window.getAttributes();
params.height = RelativeLayout.LayoutParams.WRAP_CONTENT;
params.width = RelativeLayout.LayoutParams.MATCH_PARENTS;
window.setAttributes(params);
window.setGravity(Gravity.BOTTOM);
```
2. 设置listview分割线
```java
android:divider="@color/greylinesetting"
android:dividerHeight="1dp"
android:headerDividersEnabled="false"
```
3. activity设置为
```java
android:theme="@android:style/Theme.NoTitileBar.FullScreen"
```
出现Error inflating <unknown>
通过动态设置activity全屏幕能解决
```java
getWindow().getDectorView.setSystemUiVisible(View.SYSTEM_UI_FLAG_FULLSCREEN)
```
