## Event Delegation
---
- Suppose if we want to remove li's by clicking on them as done previously where we added li's by adding inputs in [[Form Events & Prevent Default]].
- Now when we write the code, we can remove the pre-existing li's as an event listener is attached to each one of them whereas for new li's there's no event listener.
- So the solution here is use something called event delegation, which just means we're going to add our event listener to parent of the li elements that is ul.
- We will make use of the target attribute in order to remove the li element, the target attribute let's us know exactly which element in the ul was clicked even though the event listener is applied on ul.