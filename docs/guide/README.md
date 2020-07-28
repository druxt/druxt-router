---
title: Introduction
---

# Druxt.js Router

The Druxt.js Router brings simple decoupled [Drupal](https://drupal.org) routing to your Nuxt.js application with the power of Drupal's JSON:API and [Vuex](https://vuex.vuejs.org).


## Features

### Nuxt.js module

The Nuxt.js module sets up a wildcard router that resolves to the Druxt.js Router component page.

The module comes with support for the Druxt.js Entity and Views modules, but also supports custom route resolvers through configuration.


### Vue component

The `<druxt-router />` component uses the Vuex store to query the Drupal JSON:API and the [Decoupled Router](https://www.drupal.org/project/decoupled_router) for route and redirect information.

After any redirects are resolved, the route's component is rendered with the required route properties.


### Vuex store

The Vuex store is used to hold all Drupal JSON:API routes, redirects, resoures and queries accessed during the active session.


### Vue mixin

The `DruxtRouterEntityMixin` provides easy integration with Druxt.js Router, including lazy loading of JSON:API resources.