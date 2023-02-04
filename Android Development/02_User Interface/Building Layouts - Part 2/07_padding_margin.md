### Padding and Margin

1. In order to add margin to a view, you need to have a viewgroup containing that particular view.
2. If you apply padding and margin on a TextView, the padding is handled by the TextView itself whereas the margin is handled by the parent viewgroup containing that TextView.
3. Example
	1. Padding
		android : padding = "8dp"
		OR
		android:paddingLeft = "8dp"
		android:paddingRight = "8dp"
		android:paddingTop = "8dp"
		android:paddingBottom = "8dp"
		The default value for padding is 0dp.
	2. Margin
		android:layout_margin="8dp"
		OR
		android:layout_marginLeft="8dp"
		android:layout_marginRight="8dp"
		android:layout_marginTop="8dp"
		android:layout_marginBottom="8dp"