   ### View Groups
 
 #### Introduction
 1. View Groups are also views and they are rectangles on the screen.
 2. They can have a width, height or the background color.
 3. The content that view groups hold are simply views, that is you can think of them as container for views or parent of views and the views are known as children of view groups.
 4. **Note :** View Groups are also a type of views, so along with ImageView, TextView, ViewGroups can also be considered as a view.

#### Types of View Groups
1. Each ViewGroup has specific rules on how it will place the children inside of it.
2. Types of View Groups
	1. Linear Layout
		- Arranges children in a vertical column or in a horizontal row.
	2. Relative Layout
		- Arranges children relative to the parent. For example to the bottom of the parent or to the top of the parent. 
		- You can also arrange children relative to the other children present in the viewgroup.
3. Example Code
```XML
	//can also set orientation as horizontal //
<LinearLayout			  
    android:orientation="vertical"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content">
 
    <TextView
        android:text="Guest List"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
		android:textSize = "24sp"/>
 
    <TextView
        android:text="Yash"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content" />
	
	<TextView
    	android:text="Sagar"
    	android:layout_width="wrap_content"
    	android:layout_height="wrap_content" />
 
</LinearLayout>
```