# 1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?
Answer:
* getElementById: This method is used to select a single element by its unique ID. IDs must be unique within an HTML document. It returns a single element object or null if no element with the specified ID is found.
* ​getElementsByClassName: This method selects multiple elements that share the same class name. It returns an HTMLCollection  of all elements that have that class. Even if only one element is found, it's still returned within this collection.
* ​querySelector: This is a more modern and versatile method that selects the first element that matches a specified CSS selector. 
​* querySelectorAll: Similar to querySelector, but it returns a NodeList of all elements that match the specified CSS selector. 

​

# 2. How do you **create and insert a new element into the DOM**?
Answer:To add a new element to the DOM, we typically follow these steps:
* ​Create the element: Use document.createElement(). 
* ​Modify the element: Set its properties, such as textContent, innerHTML, className, or id.
* ​Find a parent element: Select an existing element in the DOM where we want to insert the new element.
* ​Append the child: Use a method like appendChild() or insertBefore() on the parent element to add the new element. The appendChild() method adds the new element as the last child of the parent.

# 3. What is **Event Bubbling** and how does it work?
Answer:Event bubbling is a form of event propagation where an event, triggered on an element, first executes on that element before "bubbling up" through its parent elements in the Document Object Model (DOM) tree. 
* Working:
​When a user interacts with a nested element (like a button inside a <div>), the event handler on the target element (the button) is triggered first. The event then propagates up to the parent <div>, where its event handler (if one exists) is triggered. This process continues up the DOM hierarchy until it reaches the <html> and <body> elements, and eventually the document and window objects. 
# 4. What is **Event Delegation** in JavaScript? Why is it useful?
Answer:
* Event delegation is a technique in JavaScript where a single event listener is attached to a parent element to manage events from multiple child elements. This approach leverages event bubbling to catch events from child elements without adding separate listeners for each child.
# 5. What is the difference between **preventDefault() and stopPropagation()** methods?
Answer:
* ​preventDefault() affects the behavior of the event.
* ​stopPropagation() affects the flow or propagation of the event.
