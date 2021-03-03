# EXPRESS MESSAGE

## Introduction

express message is a library that was created to make it easier to write repetitive json responses, to avoid smiliar block of code


## Installation

```sh
$ npm install @codernoob/express-message
```

```js
const { notFoundHandler, errorHandler } = require('@codernoob/express-message')

// using as middleware for not found response
app.use(notFoundHandler)

// using as middleware for error handler response
app.use(notFoundHandler)

//
```

