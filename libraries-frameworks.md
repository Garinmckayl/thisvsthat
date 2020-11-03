# Libraries and Frameworks

Table of Contents
=================

   * [React vs Vue](#React-vs-Vue)
   * [Svelte vs React](#Svelte-vs-React)
   * [Next vs Nuxt](#Next-vs-Nuxt)


## React vs Vue
React is an open-source JavaScript library for building user interfaces or UI components.
Vue.js is an open-source model–view–viewmodel JavaScript framework for building user interfaces and single-page applications.

```React Class Component
class MyReactComponent extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
}
```
<!-- tabs:start -->

#### ** React **

```javascript
class MyReactComponent extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
}
```

#### ** Vue **

```javascript
class MyVueComponent extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
}
```

<!-- tabs:end -->

## Svelte vs React
Svelte is an open-source Javascript framework, Svelte writes code that surgically updates the DOM when the state of your app changes.
React is an open-source JavaScript library for building user interfaces or UI components.


```Svelte Component
<script>
	let name = 'world';
</script>

<h1>Hello {name}!</h1>
```


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