# Cocoon-js
Contains the Javascript dependency for the [cocoon](https://github.com/nathanvda/cocoon) rubygem. 

# Why 
The existing gem has a dependency on JQuery that requires you loading JQuery manually via the asset pipeline. JQuery is no longer added by default in Rails 5, and manually adding it back breaks some `rails-ujs` functionality. This package contains the [cocoon.js](https://github.com/nathanvda/cocoon/blob/master/app/assets/javascripts/cocoon.js) code, and installs jQuery via npm

# How to use 
- Install the [cocoon] rubygem as usual
- In a JS file that relies on the cocoon javascript, import `cocoon-js` at the top of the file

For example, if you're using webpacker and have an `application.js` entrypoint, you can do:
```js
// app/javascript/packs/application.js
import "cocoon-js";
...

```