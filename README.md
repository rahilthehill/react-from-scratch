# React app created from scratch
[Threejs-Journey-Lesson-41](https://threejs-journey.com/lessons/first-react-application#)

## NOTES

### Process
1. Create a nodejs project
2. Use terminal to run npx command 
`npm init -y`
3. Creates a package.json
4. Force using specific versions of dependencies
5. If there are vulnerability warnings, you can ignore it.
6. for future projects (own), use the latest version
`npm install "dependancy"@latest`
7. 3 dependencies needed (Forced versions here)
`npm install react@18 react-dom@18.2 react-scripts@5.0`
react - core of react
react-dom - a DOM renderer for react
react-scripts- common scripts for building/servers/production
8. these are updated in the scripts section in the package.json
9. Two scripts needed, to start the local server and building for production
10. in the package.json, go the the scripts tag and add
`"dev": "react-scripts start",` and `"build": "react-scripts build"`
11. the "dev" can be either start or dev or any name really. 
12. Need to create then a public folder, this will contain files we want to be availble as they are, basically the "static" folder, it's public for react.
13. Create a `index.html` file in there
14. Change the title (lesson instruction)
15. Creating a div with `<div id="root"></div>`, this will contain the react application, the id used for targetting it
16. create the SRC folder
17. this contains the source files, which are processed before getting output as classic web-friendly content,javascript is inside, with CSS, and etc....
18. create the `index.js` file in the src folder
19. now in the index.js file, add `import { createRoot } from 'react-dom/client'` this createRoot adds and creates the roof of a ReactDOM application
20. Pass the id root div inside, call it using the function, `const root = createRoot(document.querySelector('#root'))`
21. Inside that root, render the method by using the render() method, `root.render(<h1> Hello React </h1>)`
22. Start it now using the terminal by running the `npm run dev`
23. This will give you a `We're unable to detect target browsers.` warning, it will ask to add defaults, when you are writing the index.js file, the code in transpilled to maximse the compatability, thus react needs to know which browsers to target to create the application web friendly. we don't really care as we are targetting modern browsers, thus, just enter `y`
24. starts the server and also adds the browser stuff into the package.json, might have to do some changes if you want to support different browsers.
25. However, using VITE intergrates very well, so use that instead :happy:

### Pros & Cons
Ever evolving react and libraries, there can be problems with dependencies and such, this is stuff with everything, you don't have to clean up things, but you do have to make sure for the versions are correct etc... 

 
