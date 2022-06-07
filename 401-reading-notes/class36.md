# React

# JSX
JSX produces React “elements”. We will explore rendering them to the DOM in the next section. Below, you can find the basics of JSX necessary to get you started.


# Rendering Elements

An element describes what you want to see on the screen:
Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.
`const root = ReactDOM.createRoot(
  document.getElementById('root')
);
const element = <h1>Hello, world</h1>;
root.render(element);`

# Components and Props
- Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. 

Rendering a Component
`function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
const root = ReactDOM.createRoot(document.getElementById('root'));
const element = <Welcome name="Sara" />;
root.render(element);`

Composing Components
- Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components.

`function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
function App() {
  return (
    <div>
      <Welcome name="Sara" />
      <Welcome name="Cahal" />
      <Welcome name="Edite" />
    </div>
  );
}`


Extracting Components
`function Comment(props) {
  return (
    <div className="Comment">
      <div className="UserInfo">
        <img className="Avatar"
          src={props.author.avatarUrl}
          alt={props.author.name}
        />
        <div className="UserInfo-name">
          {props.author.name}
        </div>
      </div>
      <div className="Comment-text">
        {props.text}
      </div>
      <div className="Comment-date">
        {formatDate(props.date)}
      </div>
    </div>
  );
}`


# Next.js

Next.js: The React Framework

Enter Next.js, the React Framework. Next.js provides a solution to all of the above problems. But more importantly, it puts you and your team in the pit of success when building React applications.
Next.js aims to have best-in-class developer experience and many built-in features, such as:

  - An intuitive page-based routing system (with support for dynamic routes)
  - Pre-rendering, both static generation (SSG) and server-side rendering (SSR) are supported on a per-page basis
  - Automatic code splitting for faster page loads
  - Client-side routing with optimized prefetching
  - Built-in CSS and Sass support, and support for any CSS-in-JS library
  - Development environment with Fast Refresh support
  - API routes to build API endpoints with Serverless Functions
  - Fully extendable
  - Next.js is used in tens of thousands of production-facing websites and web applications, including many of the world's largest brands.