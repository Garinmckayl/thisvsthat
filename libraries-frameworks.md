# Libraries and Frameworks

Table of Contents
=================

   * [React vs Vue](#React-vs-Vue)
   * [Svelte vs React](#Svelte-vs-React)
   * [Jquery vs React](#Jquery-vs-React)
   * [Next vs Nuxt](#Next-vs-Nuxt)
   * [Bootstrap vs Material](#Bootstrap-vs-Material)
   * [Bootstrap vs Tailwind](l#Bootstrap-vs-Tailwind)


## React vs Vue
React is an open-source JavaScript library for building user interfaces or UI components. 

Vue.js is an open-source model–view–viewmodel JavaScript framework for building user interfaces and single-page applications.

#### **Basic Component**
<!-- tabs:start -->

#### ** React **

```javascript
// react class based Component
class MyReactComponent extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
}

// function based Component
function MyReactComponent() {
  return <h1>Hello world</h1>;
}
```

#### ** Vue **

```javascript
<template>
  <h1>Hello World</h1>
</template>
<script>
  export default {
    name: "MyVueComponent",
  };
</script>
```

<!-- tabs:end -->

## Svelte vs React
Svelte is an open-source Javascript framework, Svelte writes code that surgically updates the DOM when the state of your app changes. 

React is an open-source JavaScript library for building user interfaces or UI components.




<!-- tabs:start -->

#### ** Sveltejs **

```javascript
<script>
	let name = 'world';
</script>

<h1>Hello {name}!</h1>
```

#### ** Reactjs **

```javascript
class MyVueComponent extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
}
```

<!-- tabs:end -->













## Jquery vs React
Svelte is an open-source Javascript framework, Svelte writes code that surgically updates the DOM when the state of your app changes. 

React is an open-source JavaScript library for building user interfaces or UI components.


<!-- tabs:start -->

#### ** Jquery **

```javascript

```

#### ** Reactjs **

```javascript
class MyVueComponent extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
}
```

<!-- tabs:end -->



## Next vs Nuxt
Next.js is a free and open source web application framework based on react.js, It allows you to build ssr applications. 

Nuxt.js is a free and open source web application framework based on Vue.js, Node.js, Webpack and Babel.js.

```Next Basic link
import Link from "next/link";
function Home() {
  return (
    <Link href="/">
      <a>Home</a>
    </Link>
  );
}
```



<!-- tabs:start -->

#### ** Nextjs **

```javascript

```

#### ** Nuxtjs **

```javascript

```

<!-- tabs:end -->









## Bootstrap vs Material Design
Bootstrap is a free and open-source CSS framework directed at responsive, mobile-first front-end web development. It contains CSS- and JavaScript-based design templates for typography, forms, buttons, navigation, and other interface components. 

Material Design is a design language that Google developed in 2014. Expanding on the "card" motifs that debuted in Google Now, Material Design uses more grid-based layouts, responsive animations and transitions, padding, and depth effects such as lighting and shadows. 





<!-- tabs:start -->

#### ** Nextjs **

```javascript

```

#### ** Nuxtjs **

```javascript

```

<!-- tabs:end -->






## Bootstrap vs Tailwind
Bootstrap is a free and open-source CSS framework directed at responsive, mobile-first front-end web development. It contains CSS- and JavaScript-based design templates for typography, forms, buttons, navigation, and other interface components.  

A utility-first CSS framework packed with classes like flex, pt-4, text-center and rotate-90 that can be composed to build any design, directly in your markup.

```html
import Link from "next/link";
function Home() {
  return (
    <Link href="/">
      <a>Home</a>
    </Link>
  );
}
```



<!-- tabs:start -->

#### ** Bootstrap **

```javascript

```

#### ** Tailwind **

```javascript

```

<!-- tabs:end -->