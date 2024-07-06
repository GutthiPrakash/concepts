# Browser Rendering

The process of browser rendering of HTML, CSS, and JavaScript involves parsing the resources into structured models (DOM tree and CSSOM), combining them into a render tree, calculating layout, painting pixels on the screen, and handling dynamic updates through JavaScript.

The stages in browser rendering : 

## 1.HTML Parsing

Initially the browser receives the HTML content from the server and starts parsing it into DOM structure.The browser breaks down the HTML into tokens like start tags, end tags, attribute names, attribute values, etc. Now the browser converts these tokens into a structured tree of elements, which becomes the DOM tree.


![image](https://github.com/GutthiPrakash/concepts/assets/138982117/66c370f9-023e-4536-834a-89dd8eb35484)



## 2.CSS Parsing and Styling

As the browser parses HTML, simultaneously the browser fetches the CSS associated with the document and parses them into CSSOM (CSS Object Model). It computes the final styles for each element based on CSS specificity rules and inheritance.

## 3.Render Tree Construction

Once the browser received both DOM tree and CSSOM, it combines them to create a render tree. this render tree contains only the elements that are going to be rendered on the screen and their computed styles.

## 4.Layout

With the created render tree, the browser calculates the exact position and size of element on the screen. At this stage the browser takes into key factors like the dimensions of the viewport, the computed styles of elements, and any dynamic changes that affect layout.

## 5.Painting

At this stage the browser paints each element onto the screen according to the information in the render tree like dimensions and styles.

## 6.JavaScript Execution

The JavaScript can directly manipulate the DOM tree, CSS styles and that leads to dynamic updates. If any changes initiated by JavaScript may require the browser to repeat the steps of rendering process to reflect the changes on the screen.

## References

* [ How browser works ](https://developer.mozilla.org/en-US/docs/Web/Performance/How_browsers_work)
* [ DOM & How Does HTML Rendering Happen in Browsers? ](https://engineering.teknasyon.com/what-is-the-dom-how-does-html-rendering-happen-in-browsers-cbeb12bdfea6)
* [ How does a browser work? ](https://youtu.be/5rLFYtXHo9s?si=1JZaqvzOWH55WFCt)
