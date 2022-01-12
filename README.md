# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).


React.JS folder structure

.env
.prettier/eslint configs
.storybook - Storybook configuration.

src
    /assets - like images, css & fonts
    /components  -  reusable atomic & molecular 
            Component.tsx
            Component.style.tsx
            Component.test.tsx
            Component.stories.tsx
            index.tsx
    /constants - Eg : Regex & other application generic constant
    /helpers - reusable helper functions
    /hooks - contain custom hooks
    /layout - layout components - the common top wrapper component 
            (usually will contain navbar, sidebar, footer and children components)
    /pages - Each component can layout component as top wrapper based on the page structure. 
            Each component exported as default, since lazy loading works with default export
    /providers - e.g. translation provider, localization
    /routes - dynamic configuration, nested array
    /schema - schema files can use yup and might be used with formik
    /service - http request, axios might be used
    /store
        /actions
        /reducers
        /selectors
        /index.tsx
    /styles - theme, global styles
    /config - contain the config file using env
    /App.js - main component - container for all components
    /index.js - contain render method
    /test.utils.tsx - It contain method to render the jest component file
This function required since we need to add top wrapper component of react-router, redux & styled-components. Without adding this wrapper component, test cases will not run.