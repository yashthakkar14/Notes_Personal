### Image View

1. src represents the source of the particular image.
2. Example
```XML
<ImageView
		   android:src = "@drawable/cake"
		   android:layout_width = "wrap_content"
		   android:layout_height = "500dp"
		   android:scaleType = "center"/>
```
3. Explanation
	1. Here cake is the file name.
	2. We use the '@' symbol to tell that we are referencing a resource in the android app.
	3. Drawable is the resource type, a graphic that will be shown on the screen in android.
	4. We have the file name in the end and don't need to mention the extension.
	5. scaleType tells the device how to scale up or scale down the image based on the bounds of the image view.
	6. scaleType : center doesn't change the size of the image, it just centres it.
	7. centerCrop scales down the image to fit the **width and height of the view** (size of the screen).
	8. We don't harm the aspect ratio and center and crop the image.