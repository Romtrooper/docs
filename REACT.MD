## Some rules to follow

### Naming

#### Naming Components

1. Name the component by it's purpose
2. Start a component name with capital letter
  * It make it easier to JSX to identify a custom component insteand of an HTML tag.
  * For example use `Menu` instead of `menu`
3. Do not name a component file name `index.js`
  * It make debugging more difficult
4. Name components in upper Camel Case => `AppLayout` instead of `applayout`

#### Components Responsability

To ensure components reusability we must avoid creating large components mixing a lot of logic and styling.

Components must be:

1. Reusable as much as possible
2. Testable
3. Easy to understand
3. Stateless when they are only displaying data



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
