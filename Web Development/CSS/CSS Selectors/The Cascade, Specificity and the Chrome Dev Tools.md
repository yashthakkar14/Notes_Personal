## The Cascade, Specificity and the Chrome Dev Tools
---
### Cascade
- The order your styles are declared in and linked to matters !
- Example : If there are more than one h1 styles in a single css file, then the one declared latest is given preference.(overrides)
- If there are two css files then the one declared latest is given preference.
---

### Specificity
- Specificity is how the browser decides which rules to apply when multiple rules could apply to the same element.
- It is a measure of how specific a given selector is. The more specific selector "wins".
- For example, if same paragraph element has two CSS selectors to color it, one is *div p* and the other is *p*, then div p will be given higher specificity even if *p* comes after *div p* as *div p* is more specific.
- ID > Class > Element. This is the order of specificity.
- Example - [[Specificity Calculator.png]]
- Specificity Calculator
	https://specificity.keegan.st
- **Note:** This doesn't work like normal number system, for example [[Comparison Specificity.png]], in this case even though there are 28 elements, the one with class will be given higher preference as it has higher specificity.
---

### Chrome Dev Tools
- CSS styles can be seen in console.
- Can help when you are not sure why a particular CSS style is not working.
- You can also try experimenting in the console by changing CSS values.

---
### Tags
#node, #selectors 