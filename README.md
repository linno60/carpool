# Carpool Application

This is an Carpool Application linking student drivers with riders, a website which drivers and passengers can use it to find each other, save time and make benifits.

## Getting Started

This README would normally document whatever steps are necessary to get the application up and running.

## Architecture

There will be two parts:
A REST API server
    - Node.js
A responsive front-end
    - AngularJS


## Documentation

## Installation

 Install [node.js]
 http://nodejs.org/
 `npm install` to install all dependencies
 Install [mysql]
 http://mysql.com and run `./sql/deploy.sh`  may need to edit the credentials in the script depending on 
  how you set up mysql

## Running Locally

 `./scripts/start-server.sh`

## Running Tests


Run  `test-client.sh` script to run all client unit tests.


Run  `test-server.sh` script to run all server unit tests.


## End-To-End Tests

Run the application locally and run the `e2e-test.sh` script to run all end-to-end tests.

In a different terminal window or tab:
`./scripts/e2e-test.sh`



## Development

Please feel free use a different markup language if you do not plan to run rake doc:app.



## The MIT License (MIT)

Copyright (c) 2015

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
