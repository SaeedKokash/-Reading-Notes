# Component-Based Architecture #

## What is a “component”? ##

A Component Architecture is about replaceable components and re-using them in different parts of a project to ensure independency, manage the complexity and making the 
components modular as much as possible. 

## Examples of Component Frameworks ##

There are many standard component frameworks such as COM/DCOM, JavaBean, EJB, CORBA, .NET, web services, and grid services.
These technologies are widely used in local desktop GUI application design such as graphic JavaBean components, MS ActiveX components, and COM components 
which can be reused by simply drag and drop operation.

## What are the characteristics of a component? ##

- Reusability − *A component is mainly reused in different situations in different applications.*
- Replaceable − *A Component may be replaced with other similar components if possible.*
- Not context specific − *A Component is designed to operate in different environments and contexts.*
- Extensible − *A component can be extended from existing components to provide new behavior.*
- Encapsulated − *A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.*
- Independent − *Components are designed to have minimal dependencies on other components.*

## What are the advantages of using component-based architecture? ##
- **Ease of deployment** − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
- **Reduced cost** − The use of third-party components allows you to spread the cost of development and maintenance.
- **Ease of development** − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
- **Reusable** − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
- **Modification of technical complexity** − A component modifies the complexity through the use of a component container and its services.
- **Reliability** − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
- **System maintenance and evolution** − Easy to change and update the implementation without affecting the rest of the system.
- **Independent** − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

## Principles of Component−Based Design ##
![](https://www.tutorialspoint.com/software_architecture_design/images/principles_of_component_based_design.jpg)

## *[Source](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)* ##

<hr>
<hr>

# What is Props and How to Use it in React#

## What is “props” short for? ##
“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)


## How are props used in React? ##

Using props is very easy in React and can be simplified by three main steps:

- **Define** an attribute and its value(data).
- **Pass** it to child component(s) by using Props.
- **Render** the Props Data.

## What is the flow of props? ##

Props are a (uni-directional) one way data flow which means that they go from a parent to a child which makes it easier to debug and more efficient.

![Uni-directional data flow chart](https://blog.openreplay.com/static/534813c989d40e3240f264b9534d2f94/0ff54/hero.jpg)

## *[Source](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)* ##

<hr>
<hr>

## Useful Resources ##

- [React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Hello world](https://reactjs.org/docs/hello-world.html)
- [React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
- [React Docs - Rendering elements](https://reactjs.org/docs/rendering-elements.html)
- [React Docs - Components and props](https://reactjs.org/docs/components-and-props.html)

<hr>
<hr>

## Things I want to know more about
