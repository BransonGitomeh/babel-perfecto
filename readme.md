i now have es6 and use babel. im using features that are in stage 2. and ar enot supported in node

but i will be transpiling down to be able to use them all over;.

this means that i now have a build folder as if i was doing minificaton and building for frontend things . and things are generally intresting 

```javascript
"scripts": {
    "start": "nodemon index.js --exec babel-node lib/index.js --presets es2015,stage-2",
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "babel lib -d dist --presets es2015,stage-2",
    "serve": "node dist/index.js"
  },
```

The more i read other people code, the more im humbled by how much i learn every day.

most code has come from following https://github.com/babel/example-node-server