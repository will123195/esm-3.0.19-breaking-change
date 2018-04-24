# esm-3.0.19-breaking-change

Tested with Node v8.9.4

#### Behavior without esm

```js
node index.js

// b.js has been loaded
```

#### Behavior using esm@3.0.18

```js
node -r esm index-esm.js

// b.js has been loaded
```

#### Behavior using esm@3.0.19+

```js
node -r esm index-esm.js

// b.js has been loaded
// b.js has been loaded
```

Notice `b.js` is loaded twice!