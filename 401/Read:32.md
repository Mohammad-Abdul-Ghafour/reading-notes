# React 3

## React Js vs Next Js

* React is a JavaScript library that helps you to build user interfaces using components as building blocks.
* Reactjs do one part of all the web app, which is to build UI components to show content.
* NextJS is a framework with a set of libraries that work together to build a web app, and one of those libraries is Reactjs

### Create a Next.js app

1. in terminal: `npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"` , you will be promt a question, type `y`. this command is creating a next app using a template
2. cd into the folder: `cd nextjs-blog`
3. run `npm run dev` to start Next.js app’s development server on `http://localhost:3000/` you will see "Welcome to Next.js!" page
4. we can see in pages -> index.js the code for the page we see when we run the server, we can change it as we like

### Creating Pages in Next.js

* In Next.js, a page is a React Component exported from a file in the pages directory.
* to create a page: create a file inside the pages folder
* inside your file add a react component with what you want
* we must export the component as default
* Now to visit your component, simply go to the server and add `/page_name`, you will see whatever you added in your component.
* Simply create a JS file under the pages directory, and the path to the file becomes the URL path.

### Link Component

* In Next.js, you use the Link Component from next/link to wrap the `<a>` tag. `<Link>` allows you to do client-side navigation to a different page in the application.
* Example:

```javascript
import Link from 'next/link'

<h1 className="title">
  Read{' '}
  <Link href="/posts/first-post">
    <a>this page!</a>
  </Link>
</h1>
```

* In the example above `{' '}` adds an empty space, which is used to divide text over multiple lines.

### Client-Side Navigation

* Client-side navigation means that the page transition happens using JavaScript, which is faster than the default navigation done by the brows

### Assets, Metadata, and CSS

* Next.js has built-in support for CSS and Sass.
* Any images or static data can be added in `public directory`
* we can add an image using the image component from next.js `import Image from 'next/image'`
* Metadata can be changes from index.js
* or in other pages by importing `import Head from 'next/head'`
* to add stylingwe can use a library called **styled-jsx**. It’s a “CSS-in-JS” library — it lets you write CSS within a React component, and the CSS styles will be scoped (other components won’t be affected).

## React Context

* used to easily share state in my applications without using props.
* Context provides a way to pass data through the component tree without having to pass props down manually at every level.
* It share global data between all components of the tree.
* global state: state in multiple components that are not directly connected.
* global context: Context is designed to share data that can be considered “global” for a tree of React components
* provider: a Provider React component that allows consuming components to subscribe to context changes.
* consumer: a Consumer React component that consumes components that is subscribed to context changes

### Context uses

* Themes
* Multilingual application
* Authorization
