<img src="screenshot.png" alt="" style="margin: 0 auto; max-width: 100%;" />


# Hello 2

Simple 'Hello World' with a Vue 2 package.

> Note: The latest Vue 2 version used here is 2.6.14.


## Run this project

### 1. Install dependencies

```
yarn
````


### 2. Preview in the browser

```
yarn start
```

> Note: The above command will open `index.html` on port 20221.


## Steps to re-create

### 1. Initialize `yarn`

Initialize `yarn` (or `npm`) and create `package.json`.

```
yarn init
````


### 2. Add dependencies

```
yarn add live-server
yarn add vue@2.6.14
```

> Note: `live-server` package is added to enable live reload functionality.


### 3. Add a Vue 2 reference in index.html

```
<script src="node_modules/vue/dist/vue.min.js"></script>
```


### 4. Add scripts

In `package.json` add the following scripts:

```
"scripts": {
  "server": "live-server --open=index.html --port=20221",
  "start": "yarn server"
}
```


### 5. Run the project

```
yarn start
```

> Note: The above command will open `index.html` on port 20221.


### 6. Add an element with id="app" in `index.html`

```
<div id="app">
  ...
</div>
```


### 7. Add a script to initialize Vue 2 app

```
<script>
  const app = new Vue({
    el: '#app',
    data: {
      hello: 'Hello World',
    },
  });
</script>
```


### 8. Display Vue 2 data within the element with id="app"

```
<div id="app">
  <h1 class="title">Welcome to Vue</h1>
  {{ hello }}
</div>
```
