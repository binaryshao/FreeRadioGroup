demo演示：

![](https://github.com/Sbingo/FreeRadioGroup/raw/master/gif/FreeRadioGroup.gif) 

### Description

 1. This is a **moveable** RadioGroup could **fade out**, and **auto return to its parent's left or right**,   it has **no side effect** to RadioGroup's setOnCheckedChangeListener method .
 
 2. Though it's a RadioGroup , the ideas used here make it very easy for you to custom your own View or ViewGroup which reacts in the similar way.

### Usage

 

 - In your root build.gradle add:

```
allprojects {
	repositories {
		...
		maven { url "https://jitpack.io" }
	}
}
```

 - Add the dependency
```
compile 'com.github.Sbingo:FreeRadioGroup:v1.0.0'
```
 
 - In the xml layout file:
 
```
 <sbingo.freeradiogroup.FreeRadioGroup
        android:id="@+id/group"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginRight="5dp"
        android:background="@drawable/black_bg"
        app:autoBack="true"           //松手后是否自动回到父布局左侧或右侧
        app:millisInFuture="2500"     //从松手到淡出的时间
        app:toAlpha="0.3"             //淡出后的透明度值
        app:moveable="true">          //是否能拖动
        <RadioButton
		    .....
            />
            .
            .
            .
        <RadioButton
		    .....
            />
</sbingo.freeradiogroup.FreeRadioGroup>

```

### If you feel it's useful, just give me a **star**, thank you~

### 公众号
![as彬哥六六六](https://s2.ax1x.com/2019/03/26/AUooOs.jpg)
