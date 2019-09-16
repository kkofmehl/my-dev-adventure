# React/Redux Intensive

Packages:
- react
- react-dom
- babel-core
- babel-loader
- babel-preset-env 
- babel-preset-es2015 
- babel-preset-react 
- babel-preset-stage-2 
- css-loader 
- webpack
- webpack-dev-server
- react-hot-loader@3.0.0-beta.7
- node-sass
- sass-loader
- style-loader

## Notes:

> All React components need to start with a Capital Letter

> 	document.querySelector()  => Similar to jQuery.  Can query the DOM using jQuery-esk convention

Notes on "state" vs "props"
- props should be considered immutable.
- state can be managed within the component
    - Always use the setState() method to change the state.

> 	Redux, in a nut-shell, is a state-management tool for React.
-	Redux https://egghead.io/courses/getting-started-with-redux



## Lifecycle Methods

> componentWillMount

The component has been created in memory but has not been rendered
(Maybe on its way out.  Most likely replaced by constructor)

>componentDidMount

This happens after the component has rendered.  Only runs in the browser.
		
>	componentWillReceiveProps

> 	componentWillUpdate

>	componentDidUpdate

### Constructor
- "constructor" is the name of the method.
- ALWAYS call the "super" within the constructor.

### Routing
            
>React-router-dom


