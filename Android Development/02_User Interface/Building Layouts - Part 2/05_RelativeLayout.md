### Relative Layout
Reference - https://developer.android.com/reference/android/widget/RelativeLayout.LayoutParams

1. Relative Layout helps you build even more flexible layouts.
2. With the relative layout, you can position the children **relative to the parent or relative to other children.**
3. Relative to parent
	1. The children inside the relative layout will be positioned relative to the parent's left, right, top or bottom edges.
	2. For example :
		```XML
		android:layout_alignParentTop = "true"
		android:layout_alignParentBottom = "false"
		android:layout_alignParentLeft = "true"
		android:layout_alignParentRight = "true"
		android:layout_centerHorizontal = "false"
		android:layout_centerVertical = "false"
		```
4. Relative to Other Views
	1. The children inside the relative layout will be positioned relative to the other children.
	2. We can assign id's to each child in order to figure them out while laying out other children with respect to them.
	3. ID example
			android:id = "@+id/ben_text_view"
			1. @refers to a resource in our android app.
			2. id is the resource type and we use '+' symbol as this is the first time we are declaring this id.
			3. Then we have '/' and then name of the view.
			4. The basic requirements are that the names can't have any spaces, it needs to start with a letter and it cannot contain any weird punctuation symbols.
	4. Align Example
			android:layout_toLeftOf = "@id/ben_text_view"
			android:layout_above="@id/jennie_text_view"
5. Padding and Margin
	1.  Padding is handled by the view itself whereas the margin is handled by the parent viewgroup.
	2.  Example
```XML
android:padding = "8dp"
android:paddingLeft = "8dp"
android:paddingRight = "8dp"
android:paddingBottom = "8dp"
android:paddingTop = "8dp"
android:layout_margin = "8dp"
android:layout_marginLeft = "8dp"
android:layout_marginRight = "8dp"
android:layout_marginTop = "8dp"
android:layout_marginBottom = "8dp"
```
6. Code Example 
	```XML
		<RelativeLayout
			xmlns:android="http://schemas.android.com/apk/res/android"
			android:layout_width="match_parent"
			android:layout_height="match_parent">

			<TextView
				android:id="@+id/lyla_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
		    android:layout_alignParentBottom="true"
				android:layout_alignParentLeft="true"
				android:textSize="24sp"
				android:text="Lyla" />

			<TextView
				android:id="@+id/me_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_alignParentBottom="true"
				android:layout_toRightOf="@id/lyla_text_view"
				android:textSize="24sp"
				android:text="Me" />

			<TextView
				android:id="@+id/natalie_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_above="@id/lyla_text_view"
				android:textSize="24sp"
				android:text="Natalie" />

			<TextView
				android:id="@+id/jennie_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_alignParentBottom="true"
				android:layout_alignParentRight="true"
				android:textSize="24sp"
				android:text="Jennie" />

			<TextView
				android:id="@+id/omoju_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_alignParentRight="true"
				android:layout_above="@id/jennie_text_view"
				android:textSize="24sp"
				android:text="Omoju" />

			<TextView
				android:id="@+id/amy_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_alignParentRight="true"
				android:layout_above="@id/omoju_text_view"
				android:textSize="24sp"
				android:text="Amy" />

			<TextView
				android:id="@+id/ben_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_alignParentTop="true"
				android:layout_centerHorizontal="true"
				android:textSize="24sp"
				android:text="Ben" />

			<TextView
				android:id="@+id/kunal_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_alignParentTop="true"
				android:layout_toLeftOf="@id/ben_text_view"
				android:textSize="24sp"
				android:text="Kunal" />

			<TextView
				android:id="@+id/kagure_text_view"
				android:layout_width="wrap_content"
				android:layout_height="wrap_content"
				android:layout_alignParentTop="true"
				android:layout_toRightOf="@id/ben_text_view"
				android:textSize="24sp"
				android:text="Kagure" />

		</RelativeLayout>
		```