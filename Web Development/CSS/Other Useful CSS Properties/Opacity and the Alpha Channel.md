## Opacity and the Alpha Channel
---
### Alpha Channel
- When we use rgba colors , for e.g (255,255,255,0.5)
- The first three values are r,g,b colors and the 4th value is alpha value which sets the transparency.
- For hexadecimal colors, opacity is set in the final two digits, for e.g #00cca000;
- Here the final two digits 00 sets the alpha channel and it ranges from 00 to FF;
- The alpha channel just works for background-color and not for other properties like text-color.
- The value ranges between 0 to 1 for alpha channel.
- Syntax
	```CSS
	#rgba{
		width:50%;
		height:50%;
		background-color:rgba(255,255,255,0.5) /*For rgba*/
	}
	```
---
### Opacity
- The opacity changes every nested element along with the element to which opacity is applied.
- Buttons, text if present in div,  div, everything changes while using opacity !
- Syntax
	```CSS
	#opacity{
		width:50%;
		height:50%;
		background-color:yellow;
		opacity:0.5
	}
	```
---
### Tags
#Other_CSS, #node 