# Vue.js with Sails.js backend example project
This project is for those who are new to [single-page applications](https://en.wikipedia.org/wiki/Single-page_application) and want to learn through a real example. Besides that, it should cover most of the features from Sails.js and Vue.js.

## Getting started
### Prerequisites
I created a [Vagrant box](https://github.com/ndabAP/Vagrant-box-with-Sails.js-Vue.js-and-MongoDB) with MongoDB, Node.js, Sails.js and Vue.js and also a [Docker file](https://github.com/ndabAP/Docker-image-with-Sails.js-vue-cli-Node.js-and-MongoDB). Or manually install Node.js and Sails.js.

#### Get Node.js

```bash
$ curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
$ sudo apt-get install -y nodejs
```

#### Get Sails.js

```bash
$ sudo npm install sails -g
```

#### Install modules

```bash
$ cd frontend && npm install
$ cd ../backend && npm install
```

### Production
First, you have to build up your Vue.js components and merge them with Sails.js. This can be done with `cd frontend && npm run build`. Now do `cd ../backend && sails lift` and then open your browser and go to [localhost:1337](http://localhost:1337).

### Development
`cd backend && sails lift` and then `cd ../frontend && npm run dev`. After that open [localhost:8080](http://localhost:8080) in your browser.

## Components used
The following components are used in this project.

### [Sails.js](https://github.com/balderdashy/sails)
This is the backend and data provider.

### [Vue.js](https://github.com/vuejs/vue)
Handle frontend data with a [MVVM](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93viewmodel).

### [Vuex](https://github.com/vuejs/vuex)
A [state pattern](https://en.wikipedia.org/wiki/State_pattern).

### [BootstrapVue](https://github.com/bootstrap-vue/bootstrap-vue)
Frontend framework. The design part.

### [vue-resource](https://github.com/pagekit/vue-resource)
HTTP client for Vue.js.

### [vue-router](https://github.com/vuejs/vue-router)
Router for the frontend.

## To do
- More tests
- more multilingualism
- file uploads
- upgrading to Sails.js 1.0
- mobile version
- finalize checkout
- use modules for Vuex

## Code style
This project fulfils the [JavaScript Standard Style](https://standardjs.com/).
