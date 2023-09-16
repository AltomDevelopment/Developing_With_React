# Getting Started with React
--- 

[Microsoft Documentation](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/react-overview)

[Installing React](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/react-on-windows)


React is an open-source JavaScript library for building front end user interfaces. Unlike other JavaScript libraries that provide a full application framework, React is focused solely on creating application views through encapsulated units called components that maintain state and generate UI elements. You can place an individual component on a web page or nest hierarchies of components to create a complex UI.

React components are typically written in JavaScript and JSX (JavaScript XML) which is a JavaScript extension that looks likes a lot like HTML, but has some syntax features that make it easier to do common tasks like registering event handlers for UI elements. A React component implements the render method, which returns the JSX representing the component's UI. In a web app, the JSX code returned by the component is translated into browser-compliant HTML rendered in the browser.

# What can you do with React?
Windows supports a wide range of scenarios for React developers, including:

- Basic web apps: If you are new to React and primarily interested in learning about building a basic web app with React, we recommend that you install create-react-app directly on Windows. If you're planning to create a web app that will be deployed for production, you may want to consider installing create-react-app on Windows Subsystem for Linux (WSL), for better performance speed, system call compatibility, and alignment between your local development environment and deployment environment (which is often a Linux server).

- Single-Page Apps (SPAs): These are websites that interact with the user by dynamically rewriting the current web page with new data from a server, rather than the browser default of loading entire new pages. If you want to build a static content-oriented SPA website, we recommend installing Gatsby on WSL. If you want to build a server-rendered SPA website with a Node.js backend, we recommend installing Next.js on WSL. (Though Next.js now also offers static file serving).

- Native desktop apps: React Native for Windows + macOS enables you to build native desktop applications with JavaScript that run across various types of desktop PCs, laptops, tablets, Xbox, and Mixed Reality devices. It supports both the Windows SDK and macOS SDK.

- Native mobile apps: React Native is a cross-platform way to create Android and iOS apps with JavaScript that render to native platform UI code. There are two main ways to install React Native -- the Expo CLI and the React Native CLI. There's a good comparison of the two on StackOverflow. Expo has a client app for iOS and Android mobile devices for running and testing your apps. For instructions on developing an Android app using Windows, React Native, and the Expo CLI see React Native for Android development on Windows.

# React Tools

While writing a simple React component in a plain text editor is a good introduction to React, code generated this way is bulky, difficult to maintain and deploy, and slow. There are some common tasks production apps will need to perform. These tasks are handled by other JavaScript frameworks that are taken by the app as a dependency. These tasks include:

- **Compilation** - JSX is the language commonly used for React apps, but browsers can't process this syntax directly. Instead, the code needs to be compiled into standard JavaScript syntax and customized for different browsers. Babel is an example of a compiler that supports JSX. [Babel Website](https://babeljs.io/)
  
- **Bundling** - Since performance is key for modern web apps, it's important that an app's JavaScript includes only the needed code for the app and combined into as few files as possible. A bundler, such as webpack performs this task for you. [Webpack Website](https://webpack.js.org/)
  
- **Package management** - Package managers make it easy to include the functionality of third-party packages in your app, including updating them and managing dependencies. Commonly used package managers include Yarn and npm.
Together, the suite of frameworks that help you create, build, and deploy your app are called a toolchain. An easy toolchain to get started with is create-react-app, which generates a simple one-page app for you. The only setup required to use create-react-app is Node.js. [NPM Website](https://www.npmjs.com/)

- For Windows development, follow the instructions to install Node.js on WSL or install Node.js on Windows. For help deciding which to use, check out the article: Should I install on Windows or Windows Subsystem for Linux?.


# React Native Component Directory

The components that can be used in a React Native app include the following:

- Core components - Components that are developed and supported as part of the React Native framework.
- Community components - Components that are developed and maintained by the community.
- Native components - Components that you author yourself, using platform-native code, and register to be accessible from React Native.

The [React Native Directory](https://reactnative.directory) provides a list of component libraries that can be filtered by target platform.

# Fullstack React toolchain options
React is a library, not a framework, so may require additional tools to create a more complex app. In addition to using React, you may want to consider using:

- Package manager: Two popular package managers for React are npm (which is included with NodeJS) and yarn. Both support a broad library of well-maintained packages that can be installed.
- [React Router:](https://reactrouter.com/en/main) a collection of navigational components that can help you with things like bookmarkable URLs for your web app or a composable way to navigate in React Native. React is really only concerned with state management and rendering that state to the DOM, so creating React applications usually requires the use of a routing library like React Router.
- [Redux:](https://react-redux.js.org) A predictable state container that helps with data-flow architecture. It is likely not something you need until you get into more advanced React development. To quote Dan Abramov, one of the creators of Redux: "Don't use Redux until you have problems with vanilla React."
- Webpack: A build tool that lets you compile JavaScript modules, also known as module bundler. When webpack processes your application, it internally builds a dependency graph which maps every module your project needs and generates one or more bundles.
- [Uglify:](https://www.npmjs.com/package/uglify-js) A JavaScript parser, minifier, compressor and beautifier toolkit.
- Babel: A JavaScript compiler mainly used to convert ECMAScript 2015+ code into a backwards compatible version of JavaScript in current and older browsers or environments. It can also be helpful to use babel-preset-env so that you don't need to micromanage syntax transforms or browser polyfills and can define what internet browsers to support.
- [ESLint:](https://eslint.org) A tool for identifying and reporting on patterns found in your JavaScript code that helps you make your code more consistent and avoid bugs.
- [Enzyme:](https://enzymejs.github.io/enzyme) A JavaScript testing utility for React that makes it easier to test your React Components' output.
- [Jest:](https://jestjs.io) A testing framework built into the create-react-app package to help with writing idiomatic JavaScript tests.
- [Mocha:](https://mochajs.org) A testing framework that runs on Node.js and in the browser to help with asynchronous testing, reporting, and mapping uncaught exceptions to the correct test cases.

# React courses and tutorials
Here are a few recommended places to learn React and build sample apps:

- The React learning path contains online course modules to help you get started with the basics.
- Build a single-page app (SPA) that runs in the browser (like this sample web app that retrieves calendar info for a user with the Microsoft Graph API)
- Build a server-rendered app with [Next.js](https://nextjs.org) or a static-site-generated app with Gatsby [Project Page](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nextjs-on-wsl)
- Create a user interface (UI) for a native app that runs on Windows, Android, and iOS devices (checkout these native Windows app samples or this sample native app that retrieves calendar info for a user with the Microsoft Graph API)
- Develop an app for Surface Duo dual-screen device
- Create a web app or native app using Fluent UI React components
- Build a React app with TypeScript

# Additional resources
- The official React docs offer all of the latest, up-to-date information on React
- Microsoft Edge Add-ons for React Developer Tools: Add two tabs to your Microsoft Edge dev tools to help with your React development: Components and Profiler.

