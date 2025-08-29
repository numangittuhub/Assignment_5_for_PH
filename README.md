# Assignment_5_for_PH
1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?

Ans:
  getElementById

Selects a single element by its unique id attribute.
Fastest among these methods because id is unique, and browsers optimize for it.
getElementsByClassName
Selects all elements that have a specific class name.
querySelector
Selects the first element that matches a CSS selector.

querySelectorAll
Selects all elements that match a CSS selector.

2. How do you **create and insert a new element into the DOM**?
Ans: 
Using document.createElement('tagName') to create a new DOM element.
Use methods like appendChild, append, prepend, insertBefore, or insertAdjacentElement to add the element to the DOM.

3. What is **Event Bubbling** and how does it work?
Ans: 
Event Bubbling: Event triggered on an element propagates up to ancestors.
How it works: Event starts at target, then bubbles up DOM tree, triggering listeners. Use event.stopPropagation() to stop.

4. What is **Event Delegation** in JavaScript? Why is it useful?
Ans:
Event Delegation: Attaching a single event listener to a parent element to handle events from its children via event bubbling.
Why Useful:
    • Performance: Fewer listeners, less memory. 
    • Dynamic Elements: Works for elements added later. 
    • Simpler Code: Centralized event handling. 

5. What is the difference between **preventDefault() and stopPropagation()** methods?
Ans:
preventDefault(): Stops an event's default action (e.g., form submission, link navigation). 
    • stopPropagation(): Stops event from bubbling up or capturing down the DOM. 
    • Difference: preventDefault affects the event's default behavior; stopPropagation affects event propagation.