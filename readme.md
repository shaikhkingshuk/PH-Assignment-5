1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?
   Ans: getElementById: It selects the element with specific id. As the id is unique, it selects only one element at a time.
   getElementsByClassName: It selects all the elements having the same specific class name. It returns HTMLcollections and it can only selects items with class name. I can't use id or tag name.
   querySelector / querySelectorAll: Both works same, but querySelector only selects the first item/element. And querySelectorAll selects all the elements with same id or tag or class name.

2. How do you **create and insert a new element into the DOM**?
   Ans. For creating I use document.createElement(). If needed first creates a div or container and then using innerHTML, I add necessary HTML to complete my task. For inserting a new element, I select it's parent and insert the item using append.child() to it's parent.

3. What is **Event Bubbling** and how does it work?
   Ans. Event bubbling is like an event, traversing through child, to parent, then grandparent and so on.
   Whenever an event listener added to a child element, it triggers the listeners not only in the child, but also triggers it's parent, then grandparent and so on. Untill it's stopped.

4. What is **Event Delegation** in JavaScript? Why is it useful?
   Ans. Event delegation is one of the outcome of event bubbling. It helps a lot when needed to use events, on multiple childs, like group of cards. I use listener to their parent. So, whenever an event performed, in a child, it's parent catch it and checks, from which child it came from and do necessary actions to complete the operations of that child.
   It saves memory, also it works dynamically on the childs, which are added later.

5. What is the difference between **preventDefault() and stopPropagation()** methods?
   Ans: preventDefault(): It mainly used to stop browser's default action. Such as it stops reloading the page while submitting a form and so on.
   stopPropagation(): It stops event bubbling. It stops the event traverse through parent, to grandparent and so on.
