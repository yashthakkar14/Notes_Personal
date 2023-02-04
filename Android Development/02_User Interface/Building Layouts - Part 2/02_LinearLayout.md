### Linear Layout

#### Introduction
1. The android:orientation attribute lets you set the orientation of the layout to vertical or horizontal.
2. The xmlns:android is the xml namespace declaration.
3. We use this namespace in order to specify that all of these attributes belong to android.
4. And therefore all of the attributes begin with 'android:' as the namespace is the shorthand for the specific url that is unique to android.
5. We can create our own custom attributes, so to prevent name conflicts we add prefix like 'android:' .
6. So basically always remember to add xml namespace declaration in the opening tag of the root view of your XML file.

#### Code
```XML
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="horizontal"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:background = "#F06292">

    <TextView
        android:text="Guest List"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="24sp"  
        android:background = "#BA68C8"/>

    <TextView
        android:text="Sagar"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="24sp"
        android:background = "#F6F423"/>
    
     <TextView
        android:text="Yash"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="24sp"
        android:background = "#F6F423"/>
    
    <TextView
        android:text="Mom"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="24sp"
        android:background = "#F6F423"/>
  
</LinearLayout>
```