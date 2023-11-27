# Introduction to React and Components

## [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.html)

## Questions

1. What is a “component”?  They are small, reusable parts of the program that each do a specific job.

2. What are the characteristics of a component?
Reusability:
Reusability reduces development time and effort by allowing components to be used in multiple contexts.

Replicability:
Replicability allows for flexibility and adaptation, enabling the system to evolve or upgrade without major disruptions.

Extensibility:
Extensibility allows developers to add new features or modify existing ones without altering the existing code.

Encapsulation:
Encapsulation hides the internal workings of a component, promoting modularity and preventing direct access to internal details.

Independence:
Independence ensures that components can function autonomously, reducing the impact of changes to other parts of the system.

3. What are the advantages of using component-based architecture?

* Easy to Use: Components make it easy to build and update software.
* Cost-Effective: It's like using ready-made LEGO pieces, saving time and money.
* Reliable: Using reliable components makes the whole program more reliable.
* Independent: Components can be developed separately, like different LEGO sets, and still work together.

## [What is Props and How to Use it in React](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

1. What is “props” short for? "Props" is short for "properties" in React. It refers to the properties or attributes that are passed from one React component to another. Props allow components to communicate and share data.
2. How are props used in React? Props are used to pass data from a parent component to a child component in React. They are defined as attributes in the parent component and then passed as arguments to the child component. The child component can access and use these props to render dynamic content.
  Example

                        // ParentComponent.js
                        class ParentComponent extends Component {
                        render() {
                            return (
                            <ChildComponent text={"I'm the 1st child"} />
                            );
                        }
                        }

                        // ChildComponent.js
                        const ChildComponent = (props) => {
                        return <p>{props.text}</p>;
                        };
                        

3. What is the flow of props? The flow of props in React is unidirectional, meaning it goes in one direction: from parent to child. Props are passed from a parent component to its child component, and any changes to the props are managed by the parent component. The child component receives and uses the props but does not modify them. This unidirectional flow helps maintain a clear and predictable data flow in React applications.

## Bookmark and Review

[React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)
[React Docs - Hello world](https://reactjs.org/docs/hello-world.html)
[React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
[React Docs - Rendering elements](https://reactjs.org/docs/rendering-elements.html)
[React Docs - Components and props](https://reactjs.org/docs/components-and-props.html)
