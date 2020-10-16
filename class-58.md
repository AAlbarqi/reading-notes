# <Login /> and <Auth />

- Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control.

- BENEFITS OF RBAC:
    - Reducing administrative work and IT support. 
    - Maximizing operational efficiency. 
    - Improving compliance. 

- Some of the designations in an RBAC tool can include:

    - Management role scope – it limits what objects the role group is allowed to manage.
    - Management role group – you can add and remove members.
    - Management role – these are the types of tasks that can be performed by a specific role group.
    - Management role assignment – this links a role to a role group.

- React-Cookies:  We can set cookies in React using the react-cookie library, it has options, you can pass in options to set expiration time.

### Terms

- global state : they are used when components need to share states. 

- global context : designed to share data that can be considered “global” for a tree of React components.

- provider : allows consuming components to subscribe to context changes. One Provider can be connected to many consumers.

- consumer : The consumer component takes a child as a function and that function returns a React node. The current context value is passed to that function as an argument.

### Resources

- [react-cookies](https://www.npmjs.com/package/react-cookies)