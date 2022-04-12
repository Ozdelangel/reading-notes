What is React context?
React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

In other words, React context allows us to share data (state) across our components more easily.

When should you use React context?
React context is great when you are passing data that can be used in any component in your application.

These types of data include:

Theme data (like dark or light mode)
User data (the currently authenticated user)
Location-specific data (like user language or locale)
Data should be placed on React context that does not need to be updated often.

Why? Because context was not made as an entire state management system. It was made to make consuming data easier.

You can think of React context as the equivalent of global variables for our React components.