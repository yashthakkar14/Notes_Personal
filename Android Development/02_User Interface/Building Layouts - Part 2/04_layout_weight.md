### Layout Weight

1. Reference - developer.android.com/guide/topics/ui/layout/linear.html
2. It is used to evenly space out children.
3. Set layout_height and layout_weight to 0dp and the weight value of 1 for each of the children.
4. Default weight value is 1 if it is not specified.
5. The process is that it would find the weight of the views and in case of 0dp, the parent will have whole height of the screen.
6. It divides the whole height of the screen by the weight sum which is 3 and then it distributes 1/3rd of the height among three text views.
7. Code
```XML
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <ImageView
        android:src="@drawable/ocean"
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_weight="1"
        android:scaleType="centerCrop" />

    <TextView
        android:text="You're invited!"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="0"
        android:textColor="@android:color/white"
        android:textSize="54sp"
        android:background="#009688" />

    <TextView
        android:text="Bonfire at the beach"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="0"
        android:textColor="@android:color/white"
        android:textSize="34sp"
        android:background="#009688" />

</LinearLayout>
```