# Redux-Additional-Info

## Redux : 

### 1. [Redux-toolkit](https://redux-toolkit.js.org/)
- The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux :
   - "Configuring a Redux store is too complicated"
   - "I have to add a lot of packages to get Redux to do anything useful"
   - "Redux requires too much boilerplate code"

### 2. [Redux Dynamic Modules](https://github.com/microsoft/redux-dynamic-modules)
- In large Javascript applications, it is often desired to perform some kind of code-splitting, so that the initial script size is small. However, in Redux, you are required to define your reducers and middleware up-front; there is no good way to dynamically add/remove these constructs at runtime.
- **redux-dynamic-modules** is designed to make dynamically loading these constructs easier. You can define a module, which contains reducers and middleware, and add it to the Redux store at runtime. We also provide a React component DynamicModuleLoader, which can load/unload modules on mount/unmount.
- Modules provide the following benefits:
  - Modules can be easily re-used across the application, or between multiple similar applications.
  - Components declare the modules needed by them and redux-dynamic-modules ensures that the module is loaded for the component.
  - Modules can be added/removed from the store dynamically, ex. when a component mounts or when a user performs an action

### 3. [Redux Saga](https://redux-saga.js.org/)
- Redux Saga is a library that aims to make application side effects (i.e. asynchronous things like data fetching and impure things like accessing the browser cache) easier to manage, more efficient to execute, easy to test, and better at handling failures.


## Additional libraries can be used :

### 1. [jwt-decode](https://github.com/auth0/jwt-decode) : 
- jwt-decode is a small browser library that helps decoding JWTs token which are Base64Url encoded.
- **IMPORTANT**: This library doesn't validate the token, any well formed JWT can be decoded. You should validate the token in your server-side logic by using something like express-jwt, koa-jwt, Owin Bearer JWT, etc.

### 2. [react-ga](https://www.npmjs.com/package/react-ga)
- React Google Analytic module

### 3. [swiper](https://swiperjs.com/)
- Swiper is a mobile touch slider with hardware accelerated transitions and amazing native behavior
- It is intended to be used in mobile websites, mobile web apps, and mobile native/hybrid apps.
