# Class 39
## Reading

## [NextJs](https://nextjs.org/learn/basics/getting-started)
- Nextjs nice with Reactjs

##3 [React Context for Beginners](https://www.freecodecamp.org/news/react-context-for-beginners/)
- React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props
- React context is great when you are passing data that can be used in any component in your application.
- These types of data include:
    
        Theme data (like dark or light mode)
        User data (the currently authenticated user)
        Location-specific data (like user language or locale)
- React context helps us avoid the problem of props drilling
- Props drilling is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it
- Example:

        import React from 'react';
        
        export const UserContext = React.createContext();
        
        export default function App() {
          return (
            <UserContext.Provider value="Reed">
              <User />
            </UserContext.Provider>
          )
        }
        
        function User() {
          return (
            <UserContext.Consumer>
              {value => <h1>{value}</h1>} 
              {/* prints: Reed */}
            </UserContext.Consumer>
          )
        }
- 
## Videos

### [Why I’m using Next.js in 2020](https://www.youtube.com/watch?v=rtgbaKBhdkk)
- Nextjs allows you to decide weather you want to render on the client side or server side 
- Allows you to develop static websites, given dynamic data
- Nextjs and Reactjs give phenomenal performance compared to other web frameworks

### [Learn useContext In 13 Minutes](https://www.youtubez.com/watch?v=5LrDIWkK_Bc)
- The context.Provider to wrap all of the code that needs access in the context
- Context is used for passing props globally
- useContext in functional components is much simpler than with class components
## Bookmark and Review

### [Next.js Examples](https://github.com/vercel/next.js/tree/canary/examples)