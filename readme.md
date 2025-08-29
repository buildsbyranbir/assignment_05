1.What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Answer:
*getElementById → one element by id.

*.getElementsByClassName → many elements by class.

*querySelector → first match using CSS selector.

*querySelectorAll → all matches using CSS selector.




2.How do you create and insert a new element into the DOM?

 Answer:
 To create and insert a new element into the DOM, first we use document.createElement() to make the element. Then we can add text or attributes to it, like using innerText or className. Finally, we put it on the webpage by using appendChild() or append(), inside a parent element such as document.body. For example, if we want to add a new paragraph, we can write:

let para = document.createElement("p");
para.innerText = "This is a new paragraph.";
document.body.appendChild(para);





3. What is Event Bubbling and how does it work?

 Answer:
 Event Bubbling means when you click on a small element, the click also goes to its parent elements. For example, if you click a button inside a div, first the button gets the click, then the div, then the body. The event “bubbles up” from child to parent automatically.




4. What is Event Delegation in JavaScript? Why is it useful?

 Answer:
 Event Delegation means we put one event listener on a parent element instead of adding listeners to many child elements. When a child is clicked, the parent detects it and runs the code. This is useful because we don’t need many listeners, it saves memory, and it works even for new elements added later.





5. What is the difference between preventDefault() and stopPropagation() methods?

 Answer:
 preventDefault() stops the browser’s default action for an element. For example, clicking a link normally opens a new page, but preventDefault() can stop that.
stopPropagation() stops the event from going up to parent elements. For example, if a button is inside a div, stopPropagation() will prevent the click from reaching the div.