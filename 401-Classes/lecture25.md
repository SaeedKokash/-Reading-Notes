# Readings: Chakra UI #

### What is a Chakra UI? ###
Chakra UI is a simple, modular and accessible component library that gives you the building blocks you need to build your React applications.

### Is Chakra UI better than material UI? ###
A core concept to be considered when comparing the two frameworks is 'Ease of Modification'.

| Chakra UI | Material UI |
| ----------- | ----------- |
| gives developers far more freedom to manipulate CSS classes of exported components and layouts and often requires less code to do so | adds far more classes to individual HTML tags related to exported components and layouts, forcing developers to fight against base styles when customizing their interface |
| provides built-in support for responsive styling without the need to create CSS classes or media queries | requires separate code to control responsive styling based on viewport changes |
| If scalable, custom designs are important for your project (which oftentimes they are), Chakra's developer convenience shines brighter than Material UI's especially as a project scales over time. | custom styling is not a major concern for your project, Material UI is beneficial as you can avoid the creation of custom components that the library provides |


### How to use Chakra UI? ###

1. install the library
``` npm i @chakra-ui/react @emotion/react @emotion/styled framer-motion ```

2. After installing Chakra UI, you need to set up the ChakraProvider at the root of your application. This can be either in your index.jsx, index.tsx or App.jsx depending on the framework you use.
```
import * as React from 'react'

// 1. import `ChakraProvider` component
import { ChakraProvider } from '@chakra-ui/react'

function App() {
  // 2. Wrap ChakraProvider at the root of your app
  return (
    <ChakraProvider>
      <TheRestOfYourApplication />
    </ChakraProvider>
  )
}
```

3. The template name for the JavaScript project is @chakra-ui. The template name for the TypeScript project is @chakra-ui/typescript.
```
# JavaScript using npm
npx create-react-app my-app --template @chakra-ui
# JavaScript using yarn
yarn create react-app my-app --template @chakra-ui

# TypeScript using npm
npx create-react-app my-app --template @chakra-ui/typescript
# TypeScript using yarn
yarn create react-app my-app --template @chakra-ui/typescript
```


### *[Source](https://chakra-ui.com/)* 
