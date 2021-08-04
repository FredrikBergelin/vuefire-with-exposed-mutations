<h1 align="center">Vuexfire + hijackable mutations</h1>

Vuexfire can now be hijacked to inject custom models to the bound documents. In your store, add the mutations and customize them 

Store:

import { walkSet } from '@fredrikbergelin/vuefire-core'

import Post from '@/models/Post' // Just an example

const VUEXFIRE_SET_VALUE = 'vuexfire/SET_VALUE'
const VUEXFIRE_ARRAY_ADD = 'vuexfire/ARRAY_ADD'
const VUEXFIRE_ARRAY_REMOVE = 'vuexfire/ARRAY_REMOVE'
const VUEXFIRE_UPDATE = 'vuexfire/UPDATE'

Mutations: 

[VUEXFIRE_SET_VALUE](state, { path, target, data }) {
  walkSet(target, path, data)
},

[VUEXFIRE_ARRAY_ADD](state, { newIndex, data, target, collectionKey }) {

  // Just an example, implement your own logic...
  
  if (collectionKey === 'posts') {
    target.splice(newIndex, 0, new Post(data))
  } else {
    target.splice(newIndex, 0, data) // Original implementation, keep only this if you want a blank slate
  }
},

[VUEXFIRE_UPDATE](
  state,
  { oldIndex, newIndex, data, target, collectionKey }
) {
  this.commit(VUEXFIRE_ARRAY_REMOVE, { oldIndex, target })
  this.commit(VUEXFIRE_ARRAY_ADD, { newIndex, data, target, collectionKey })
},

[VUEXFIRE_ARRAY_REMOVE](state, { oldIndex, target }) {
  return target.splice(oldIndex, 1)[0]
},

<p align="center"><a href="https://vuefire.vuejs.org" target="_blank" rel="noopener noreferrer"><img width="100" src="https://vuefire.vuejs.org/vuefire-logo.svg" alt="VueFire logo"></a></p>

<h1 align="center">Vuefire & Vuexfire</h1>
<p align="center">
  <a href="https://circleci.com/gh/vuejs/vuefire"><img src="https://badgen.net/circleci/github/vuejs/vuefire" alt="Build Status"></a>
  <a href="https://codecov.io/github/vuejs/vuefire"><img src="https://badgen.net/codecov/c/github/vuejs/vuefire" alt="Build Status"></a>
</p>

> Synchronize your data and Firebase Cloud Store database in real-time

Note: This version currently supports Vue 2 and Firebase 7. Support for Vue 3 / Composition API and Firebase 8 is on the way.

[**Documentation**](https://vuefire.vuejs.org)
