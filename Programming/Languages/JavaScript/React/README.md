Why React?
* Simple syntax
* Requires only vanilla JavaScript in places other UI solutions would require unique HTML templating syntax.
* JSX is an extension that can be used with React that interprets HTML syntax as HTML code.
* React is used and maintained by Facebook giving it tons of documentation and polish.
* React uses JavaScript to create UI for not only web apps, but for mobile apps, desktop apps, and VR as well.
* React is one library and not a framework, meaning it's lightweight and not very strict / doesn't force as many design patterns as a framework.
* React's virtual DOM's diffing algorithm represents the DOM in RAM (aka virtual memory) as to make comparisons with the actual DOM upon receiving updates. The diffing algorithm allows for React to intelligently update only the necessary DOM components and thus the entire DOM doesn't have to be updated / replaced WITHOUT imperative logic. This can all be done with pure declarative programming which in turn requires less code. In other words, no need to manually target specific componenets to be updated.