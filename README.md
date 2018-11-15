# 欢迎使用 TvTabLayout [ ![Download](https://api.bintray.com/packages/zhousuqiang/maven/tv-tablayout/images/download.svg) ](https://bintray.com/zhousuqiang/maven/tv-tablayout/_latestVersion)

群   号：484790001 [群二维码](https://github.com/zhousuqiang/TvRecyclerView/blob/master/images/qq.png)

>* 针对TV端的特性对TabLayout进行了适配与开发;
>* 支持图片或颜色值作为Indicator;

### 效果

![](https://github.com/zhousuqiang/TvTabLayout/blob/master/images/tv_tablayout.gif)

### Android Studio 集成

```java
implementation 'com.owen:tv-tablayout:1.0.0'
```

### 自定义属性
| 属性      |  值/类型  |  简介  |
| -------- | :-----: | :---- |
| tabIndicatorResId     | reference |   指示器的资源(图片或颜色)     |
| tabIndicatorWidth     | dimension |   指示器的宽    |
| tabIndicatorHeight     | dimension |   指示器的高     |


### 使用

```java
// 代码动态添加tab
TvTabLayout mTabLayout = findViewById(R.id.tablayout);
for(int i=0; i<15; i++) {
    mTabLayout.addTab(mTabLayout.newTab().setText("标题"+i), i == 0);
}

// 布局直接指定tab
<com.owen.tab.TvTabLayout
        android:id="@+id/tablayout3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="60dp"
        app:tabIndicatorResId="@drawable/zx_p1_light"
        app:tabIndicatorWidth="108dp"
        app:tabIndicatorHeight="15dp"
        app:tabIndicatorBackgroundColor="@color/color_88ff804B"
        app:tabIndicatorBackgroundHeight="3dp"
        app:tabMinWidth="160dp"
        app:tabScrollMode="fixed"
        app:tabGravity="center"
        app:tabPaddingBottom="12dp"
        app:tabTextSelectedScale="1.2"
        app:tabTexSize="22sp"
        app:tabTextColor="@drawable/selector_tab_font_color">

        <com.owen.tab.TabItem
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="标题1"/>

        <com.owen.tab.TabItem
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="标题2"/>

        <com.owen.tab.TabItem
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="标题3"/>

    </com.owen.tab.TvTabLayout>
```

### 更详细的使用请见exmaple

------

### 其它作品

焦点框框架[TvFocusBorder](https://github.com/zhousuqiang/TvFocusBorder)

TvRecyclerView框架[TvRecyclerView](https://github.com/zhousuqiang/TvRecyclerView)

作者 [owen](https://github.com/zhousuqiang)