# EXPRESS MESSAGE
[![Maintainability](https://api.codeclimate.com/v1/badges/fa7ff692fc39eb14c1d4/maintainability)](https://codeclimate.com/github/firmanJS/express-message/maintainability) 
Global message library for custom response and error handling
## Introduction

express message is a library that was created to make it easier to write repetitive json responses, to avoid smiliar block of code


## Installation

```sh
$ npm install @codernoob/express-message
```
### using as middleware
```js
const { notFoundHandler, errorHandler } = require('@codernoob/express-message')

// using as middleware for not found response
app.use(notFoundHandler)

// using as middleware for error handler response
app.use(notFoundHandler)
```
### using for pagination result
```js
const { getResponse } = require('@codernoob/express-message')

// using as middleware for not found response
/**
 *
 *
 * @param {*} req
 * @param {*} res
 * @param {*} data
 */
getResponse(request, response, data)

```

(The MIT License)

Copyright (c) 2019-2020 Firman Abdul Hakim

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.