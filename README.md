

# React.JS folder structure

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
    
    /styles - theme, global styles
    
    /config.ts - contain the config file using env
    
    /App.ts - main component - container for all components
    
    /index.ts - contain render method
    
    /test.utils.tsx - It contain method to render the jest component file  - This function required since we need to add top wrapper component of react-router, redux & styled-components. Without adding this wrapper component, test cases will not run.
