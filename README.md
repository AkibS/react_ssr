# react_ssr
Simple Expample for Server Side Rendering using react 

to run this project

npm install 
npm run build
npm run start

# What is server side rendering?
The most common use case for server-side rendering is to handle the initial render when a user (or search engine crawler) first requests our app. When the server receives the request, it renders the required component(s) into an HTML string, and then sends it as a response to the client

# What’s the difference between client-side rendering and server-side rendering?

In Client-side rendering, your browser downloads a minimal HTML page. It renders the JavaScript and fills the content into it.

Server-side rendering, on the other hand, renders the React components on the server. The output is HTML content.

You can combine these two to create an isomorphic app.

# Flow of CSR and SSR

<img src="https://github.com/AkibS/react_ssr/blob/master/media/1_CRiH0hUGoS3aoZaIY4H2yg.png" width="500"/>

<img src="https://github.com/AkibS/react_ssr/blob/master/media/1_jJkEQpgZ8waQ5P-W5lhxuQ.png" width="500"/>


The main difference is that for SSR your server’s response to the browser is the HTML of your page that is ready to be rendered, while for CSR the browser gets a pretty empty document with links to your javascript. That means your browser will start rendering the HTML from your server without having to wait for all the JavaScript to be downloaded and executed. In both cases, React will need to be downloaded and go through the same process of building a virtual dom and attaching events to make the page interactive — but for SSR, the user can start viewing the page while all of that is happening. For the CSR world, you need to wait for all of the above to happen and then have the virtual dom moved to the browser dom for the page to be viewable.

# When to use SSR?

1. SEO
2. Improve performance

# Cons of SSR
-SSR can improve performance if your application is small. But it can also degrade performance if it is heavy.
-It increases the complexity of the application.


referred folllowing blogs:
1. https://medium.freecodecamp.org/server-side-rendering-your-react-app-in-three-simple-steps-7a82b95db82e
2. https://medium.com/walmartlabs/the-benefits-of-server-side-rendering-over-client-side-rendering-5d07ff2cefe8


