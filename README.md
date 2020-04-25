# Vue Sharethis

A simple Vue wrapper component for sharethis.com social share widget

Sharethis.com website: https://sharethis.com

```
npm install vue-sharethis
```

OR

```
yarn add vue-sharethis
```

## Install globally:

```
import Vue from 'vue'
import Sharethis from 'vue-sharethis'

Vue.use(Sharethis)
```

## Install locally:

```
import Sharethis from 'vue-sharethis';

export default {
  name: "App",
  components: {
    Sharethis
  }
};
```

## Usage:

```
<Sharethis
      share-this-embed-url="//platform-api.sharethis.com/js/sharethis.js#property=[your-id]&product=sticky-share-buttons&cms=sop"
    />
```

## Usage with Nuxt:

```
<client-only>
  <Sharethis
        share-this-embed-url="//platform-api.sharethis.com/js/sharethis.js#property=[your-id]&product=sticky-share-buttons&cms=sop"
      />
</client-only>
```

## Properties

**share-this-elementid** - An element gets injected into the DOM with the embedded script below, it will have a unique ID, which will be used if you want the social share to only be displayed on certain pages.

**share-this-embed-url** (required) - The embed URL you can get on the sharethis.com website

**url** (optional - default: window.location.href) - The URL you want to share, you can leave it out if you don't want to share a different URL than what is being used.

This is very basic for what I needed. Feel free to message me or do push a pull request to add more functionality
