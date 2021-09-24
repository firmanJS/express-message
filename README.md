# EXPRESS MESSAGE
[![Maintainability](https://api.codeclimate.com/v1/badges/fa7ff692fc39eb14c1d4/maintainability)](https://codeclimate.com/github/firmanJS/express-message/maintainability) 
[![Test Coverage](https://api.codeclimate.com/v1/badges/fa7ff692fc39eb14c1d4/test_coverage)](https://codeclimate.com/github/firmanJS/express-message/test_coverage)
[![Publish package nodejs](https://github.com/firmanJS/express-message/actions/workflows/npm-publish.yml/badge.svg)](https://github.com/firmanJS/express-message/actions/workflows/npm-publish.yml)
## Introduction

express message is a library that was created to make it easier to write repetitive json responses, to avoid smiliar block of code for your api

## Installation

```sh
$ npm install express-message
```
### using as middleware
```js
const { notFoundHandler, errorHandler } = require('express-message')

// using as middleware for not found response
app.use(notFoundHandler)

// using as middleware for error handler response
app.use(errorHandler)
```
### using for pagination result
```js
const { getResponse, successResponse, customResponse } = require('express-message')
/**
 *
 *
 * @param {*} request
 * @param {*} response
 * @param {*} data
 */
getResponse(request, response, data)

/**
 *
 *
 * @param {*} response
 * @param {*} message
 * @param {*} data
 */
successResponse(response, message, data)

/**
 *
 *
 * @param {*} response
 * @param {integer} code
 * @param {*} message
 * @param {array} data
 */
customResponse(response, code, message, data)
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