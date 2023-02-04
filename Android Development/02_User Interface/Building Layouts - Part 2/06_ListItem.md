### List Item with Relative Layout
```XML
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent" >

    <ImageView
        android:id="@+id/image"
        android:layout_width="56dp"
        android:layout_height="56dp"
        android:scaleType="centerCrop"
        android:src="@drawable/ocean" />

    <TextView
        android:id="@+id/title"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop = "true"
        android:layout_toRightOf = "@id/image"
        android:text="Pebble Beach"
        android:textAppearance="?android:textAppearanceMedium"
        />

    <TextView
        android:id="@+id/location"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_toRightOf = "@id/image"
        android:layout_below="@id/title"
        android:text="California"
        android:textAppearance="?android:textAppearanceSmall" />

    <TextView
        android:id="@+id/distance"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_toRightOf = "@id/image"
        android:layout_below="@id/location"
        android:text="10 miles away"
        android:textAppearance="?android:textAppearanceSmall" />

</RelativeLayout>
```