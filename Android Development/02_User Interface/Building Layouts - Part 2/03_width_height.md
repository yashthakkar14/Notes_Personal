### Width and Height

#### Introduction
1. Different widths on child views.
	1. dp
	2. wrap-content
	3. match-parent
2. Different heights on child views
	1. dp
	2. wrap-content
	3. match-parent
3. If you give the width and height of match parent to the layout, the parent in this case for the layout would be the android device screen.
4. Everytime you see an attribute with 'layout_' i.e layout_height or layout_width , these are actually view group layout parameters.
5. These are used by the parent viewgroup to determine the size and position of these views.
6. Meanwhile, the other attributes like background, textSize and text are handled by the TextView view in terms of styling its own view. 

#### Code
```XML
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="horizontal"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:background="@android:color/darker_gray">

    <TextView
        android:text="VIP List"
        android:layout_width="wrap_content"
        android:layout_height="match_parent"
        android:background="#FCAF50"
        android:textSize="24sp" />

    <TextView
        android:text="Kunal"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#A5AF50"
        android:textSize="24sp" />

    <TextView
        android:text="Kagure"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#ACCF50"
        android:textSize="24sp" />

    <TextView
        android:text="Lyla"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#4CAF50"
        android:textSize="24sp" />

</LinearLayout>
```