## Why React Functional Components are the future?

A few months ago, React launched its new documentation; [React Docs Beta](https://beta.reactjs.org/) emphasizing Functional Components. It was a great move by the team, as we already know that React Functional Components are the future, since the introduction of Hooks in version 16.8.

Before the advent of Hooks, the Class component was the main hero of React and they were used every time it came to building complex apps. We have to dig deep into the origin of React and the history of both of these components to find out what caused the downfall of Class Components and how Functional Components became the most obvious choice for building React apps today.


## The React Origin Story

React was introduced to the world in May 2013 at a [JavaScript conference](https://blog.logrocket.com/history-of-frontend-frameworks/) in the US. It proved to be a game-changer and quickly became the king of JavaScript libraries. It was brought into existence by [Jordan Walke](https://twitter.com/jordwalke), a software engineer at Facebook. He also created [FaxJS](https://github.com/jordwalke/FaxJs) in 2011, the early prototype of React.

%[https://youtu.be/GW0rj4sNH2w]

Before the introduction of React, [web applications](https://hackernoon.com/react-vs-javascript-why-react-web-apps-are-better-than-plain-websites) were built using templates or HTML directives. What React did https://reactjs.org/blog/2013/06/05/why-react.html was to break the whole user interface into several small components which when put together completed the UI of the app.

In the last decade, many front end frameworks came into existence and so far, React has not only survived but thrived, effectively defeating every other framework both in usage and popularity.


![ckytuau-9-f-00-fj-0-as-69-gjmax-7-q (1).jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1644842417939/Y50PAnnmv8.jpeg)
**A comparison of major Front-End frameworks in popularity in the last 5 years.**

According to Statista, React was the [most used](https://www.statista.com/statistics/1124699/worldwide-developer-survey-most-used-frameworks-web/) web framework among developers worldwide in 2021 with a total share of 40.14% leaving jQuery behind with 34.43%.

## What are Class Components?

As discussed earlier in the article, a component in React is a piece of code responsible for rendering a certain section of the user interface. There are two types of components-

- Class Component

- Functional Component

Class Component uses ES6 JavaScript class to create a component. It was the most common way to build React apps before the introduction of Hooks in version 16.8.

``` 
import React from "react"; 

class App extends React.Component {
  render() {
    return <h1>I am Class Component</h1>;
  }
}
export default App;
```

To create a class component, you have to create a class that extends React.Component and has a render() function. Inside the render(), you can return your [JSX](https://hackernoon.com/whats-the-deal-with-jsx-9ab2f862bf2b) as usual.

Class components also have access to props, state and various lifecycle methods like:

- componentWillMount

- componentDidMount

- componentWillReceiveProps

- shouldComponentUpdate

- componentWillUpdate

- componentDidUpdate

- componentWillUnmount

Every component has a lifecycle which has [three main phases](https://www.w3schools.com/react/react_lifecycle.asp):

1. Mounting

2. Updating

3. Unmounting

The process of loading components into DOM is known as Mounting. When the component undergoes some changes and updates itself, it’s known as Updating. Unmounting is when you remove a certain component out of DOM.

All lifecycle methods are used to interact with the component at various stages of its lifecycle.

## What are Functional Components?

A Functional Component is a type of component that uses JavaScript function to create React component.

````
import React from "react";

function App() {
    return <h1>I am a Functional Component</h1>;
}
export default App;
```

To create a functional component you have to declare a function just as you do it in JavaScript.

The above snippet is an example of a functional component, it’s the written version of the class component we saw above. You can also use the ES6 Arrow functions to create a component.

```
import React from "react";

const App = () => {
    return (
       <h1>
          I am a Functional Component created with ES6 arrow function       
       </h1>
)}

export default App;
```

You can compare both types of components and can see for yourself that functional components have simpler and cleaner syntax.

But syntax isn’t always enough to jump into certain technologies, you also need a strong set of features and capabilities to build complex apps, all of which functional components lacked initially.

So in theory, developers can use class components or functional components, whatever they prefer. But in reality, only class components were capable enough to build complex features and apps leaving developers no choice apart from them.

## The Rise of Functional Components

Everything changed after React Conf 2018 where “Sophie Alpert and Dan Abramov introduced Hooks, followed by Ryan Florence demonstrating how to refactor an application to use them.” (from [React Docs](https://reactjs.org/docs/hooks-intro.html#video-introduction))

%[https://youtu.be/dpw9EHDh2bM]

The motivation behind the introduction of Hooks in functional components was to solve the problems “encountered over five years of writing and maintaining tens of thousands of components. ” (from [React Docs](https://reactjs.org/docs/hooks-intro.html#motivation))

> With hooks we separate code not based on the lifecycle method name but based on what the code is doing” - Dan Abramov

The reason why hooks got so much attention was because it brought the power of state and lifecycle methods into functional components. You now have useState hook to tackle the setState method and useEffect was capable enough to replace many lifecycle methods. No more dependency on class components.


![React functional components vs class components](https://cdn.hashnode.com/res/hashnode/image/upload/v1644844049013/ApaYG3yin.jpeg)

> If you’re familiar with React class lifecycle methods, you can think of useEffect Hook as componentDidMount, componentDidUpdate, and componentWillUnmount combined.
> 
> [React Docs](https://reactjs.org/docs/hooks-effect.html)

There are a total of 10 built-in hooks which were shipped in version 16.8. -

- useState

- useEffect

- useContext

- useReducer

- useCallback

- useMemo

- useRef

- useImperativeHandle

- useLayoutEffect

- useDebugValue

Not all of these hooks are frequently used, most of the time we need only useState and useEffect. However, if these 10 hooks are not enough for you, React also gives you the option to build your own [custom hook](https://reactjs.org/docs/hooks-custom.html).

## The Future of Class Components

We already discussed how the importance of class components diminished after hooks came into being. However, class components are not going away, at least not anytime soon. The React team themselves has mentioned that there are no current plans to remove class components from React.

There are a great number of legacy projects which still use class components but React’s team recommends using functional components for all newer projects. All the modern React tutorials also focus only on functional components. Furthermore, the introduction of new beta documentation by the React team also confirms their future vision of Hooks playing a major role in the development of future React applications.

## Conclusion

This article was a historical analysis of React. It also looks at how the Functional Component beat Class Component to become the key player in the development of React applications, despite being introduced as a low power building component that can render more or less only static applications sprinkled with some props.

If you like this article, share it on your social accounts. Check out my [blog](https://fullstackstage.com/) and follow me on [Twitter](https://twitter.com/ashutoshmishrae) if you don’t want to miss more articles just like this one.