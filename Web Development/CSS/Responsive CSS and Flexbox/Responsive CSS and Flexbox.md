## Flexbox
---
### Intro
---
- Flexbox shrinks or expands depending upon the size of the container.
- In Flexbox, there are two axes, that is the main axis and the cross axis. 
- By default the main axis goes from left to right.
- There's also a cross axis as shown in the figure.
- Cross axis depends on the main axis, that is, if main axis is horizontal, then the cross axis is vertical and vice-versa.
- ![[Flexbox Axis.png]]
---
### Flex Direction
---
- Flex direction helps us to **change the main axis direction**.
- Default is flex direction : row in which the main axis goes from left to right.
- row-reverse : makes main axis go from right to left.
- column : main axis goes from top to bottom.
- column-reverse : main axis goes from bottom to top.
---
### Justify Content
---
- Determines **how the content is distributed across the main axis**.
- The default is flex-start.
- There are other options like flex-end, center, space-between and space-around, space-evenly.
---
### Flex Wrap
---
- Wraps the content in the flex container.
- flex-wrap : wrap is used to wrap the content in the container.
- flex-wrap : wrap-reverse is used to reverse wrap the content, that is the main axis will stay the same but the cross axis will change.
- flex-wrap : nowrap does not wrap the content. 
---
### Align Items
---
- Used to distribute items along the cross axis.
- The default value here, just like justify-content is flex-start.
- The different values here are flex-start, flex-end, center, baseline.
- Baseline is basically drawing a line at the bottom of each letter and the items are aligned in that particular manner when aligned as baseline.
---
### Align Content
---
- Used to distribute space along the cross axis only when we have multiple rows or columns depending on the main axis.
- If the main axis has column layout , align content  controls the space between the rows and for rows layout it controls the space between the rows.
- It has values like flex-start, flex-end, center, space-between, space-around
---
### Align Self
---
- It is very similar to align items except that we apply this property to individual items.
- Aligns items to relative to the cross axis.
- It aligns the individual items selected and not rows and colums.
---
### Flex-Basis
---
- Defines the initial size of an element before additional space is distributed.
---
### Flex-Grow
---
- Controls the amount of available space an element should take up. Accepts a unit-less number value.
- Can use max-width and min-width to control the maximum or minimum amount of width an element can take.
- Can define the growing ratio in unit less number.
- Only grows if there is space available.
---
### Flex-Shrink
---
- If items are larger than the container, they shrink according to flex-shrink.
- Same concept as flex-grow
---
### Flex
---
- Single property to control all values.
- Works in the following order : 
- flex : grow shrink basis
---

<br>

## Media Queries
---
### Intro 
- Media Queries allow us to modify our styles depending on particular parameters like screen width or device type.
- They are used to restlyle website with respect to different sizes, that is they are used for responsive design.
- Syntax
	```CSS
		@media (min-width : 800px) and (max-width : 1000px){
			h1{
				color : purple;
			}
		}
	```
- The width, min-width and the max-width here is the width of the viewport. A viewport represents an area in computer graphics that is currently being viewed. 
- There are other parameters as well such as orientation. E.g
	```CSS
	@media screen and (orientation : landscape){
		h1{
			color : magenta;
		}
	}
	```
- The standardized sizes are 576px, 768px, 992px, 1200px
