## Some rules to follow

[Thinking with React](https://reactjs.org/docs/thinking-in-react.html)

### Components Creation

#### Naming Components

1. Name the component by it's purpose
2. Start a component name with capital letter
  * It make it easier to JSX to identify a custom component insteand of an HTML tag.
  * For example use `Menu` instead of `menu`
3. Do not name a component file name `index.js`
  * It make debugging more difficult
4. Name components in upper Camel Case => `AppLayout` instead of `applayout`

#### Single Responsibility

To ensure components reusability we must avoid creating large components mixing a lot of logic and styling.

Following the single responsibility principle, a component should as much as possible only do one thing:

See: 
[Single Responsibility Principle](https://en.wikipedia.org/wiki/Single-responsibility_principle)

Components must be:

1. Reusable as much as possible
2. Testable
3. Easy to understand
4. Stateless when they are only displaying data

If the component is gowing to grow or need some more complexity split it into multiple one following all previous principles exposed.

#### Containers

Creating containers is a great way to avoid mixing logic and rendering aspects;


#### Dealing with props

1. Destructure your props

```javascript
function Hello({ name }) {
  return <h1>Hello, {name}</h1>;
}
```

```javascript
class Hello extends React.Component {
  render() {
    const { name } = this.props;
    return <h1>Hello, {name}</h1>;
  }
}

```
It make the component much easier to read, specially when a lot of props are given;

2. Avoid unnecessary tag wraping

=> Could be used if some style want to be applied or a specific semantic tag:

```javascript
function Hello({ name }) {
  return (
   <header>
     <h1>Hello, {name}</h1>;
     <p>It's a beautiful day</p>
    </header>
  )
}
```

=> Of no semantic tag is required or no specific style is going to be applied prefer this:

```javascript
function Hello({ name }) {
  return (
   <React.Fragment>
     <h1>Hello, {name}</h1>;
     <p>It's a beautiful day</p>
    </React.Fragment>
  )
}
```

#### Styling Components


```javascript
   <MyComponent className='MyComponent' />
```

```css
.MyComponent {
    // rules here for component
}
```

## Folders

### Creating folders in a React project


#### Project folder

```
src/
├── assets/
├── components/
├── libs/
└── modules/
```

#### Component folder

```
component/
├── Component.jsx
├── Component.css
└── ComponentContainer.js
```
All files related to a component and only one must be found in it's folder

```
component/
├── button 
    ├── ComponentButton.jsx
    ├── ComponentButton.css
├── Component.jsx
├── Component.css
└── ComponentContainer.js
```

#### Module folder

```
component/
├── ComponentClient.js
├── ComponentActions.js
├── ComponentConstants.js
└── ComponentReducer.js
```
