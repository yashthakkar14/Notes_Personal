**Note : Refer the below code for the example**

#### Wrap Content
- We can set width or height as 'wrap_content' in android where the width or the height will be set **based on the width or height of the content present in the view and change itself accordingly.**

#### Text Size
- We can set the textsize in XML too just as font-size in HTML. 
- The unit for the text size is **sp** which stands for scale independent pixels which changes across devices depending on the resolution of that particular device.
- You can also set the size as 
androidTextAppearance = "?androidTextAppearanceLarge"/>

#### Background Color
- There are a limited set of colors provided by android itself.
- So you can specify exact hexadecimal color in order to give the desired background color to your view.

#### Text Style
- We can also add text style like changing our text to italic, bold or allcaps, etc.

#### Code Example
```XML
<TextView
    android:text="Excited for the gift you'll surprise me with."
	android:background="@android:color/blue"
    android:background="#7E57C2"
    android:textColor = "#FFF59D"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:textSize = "20sp"
    android:textAppearance="?android:textAppearanceLarge"
	android:textStyle = "bold"
	android:textAllCaps = "true"
/>
```