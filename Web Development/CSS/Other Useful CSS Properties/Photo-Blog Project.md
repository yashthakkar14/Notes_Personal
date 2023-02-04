## Photo-Blog Project
---

### Key Takeaways
- We can give width to images.
- We can add margin to seperate those images with the help of calculation.
- We can either calculate them manually or
- We can ask CSS to calculate it using calc property.
- Example
	```CSS
		margin : calc(10%/6)
	```
- When you enter images in different lines together, there's a whitespace created between those images for e.g
	```CSS
	<img src = "img.jpg">
	<img src = "img.jpg">
	<img src = "img.jpg">
	```
- Whereas if you do it like below, there would be no space created
	```CSS
	<img src = "img.jpg"><img src = "img.jpg"><img src = "img.jpg">
	```
- The reason is that because of the whitespan, the same issue is with inline elements with span too.
- In case of flexbox there would be no such issues, but in case of very specific calculations, this issue might be encountered.

---

### Tags
#Other_CSS , #node #position