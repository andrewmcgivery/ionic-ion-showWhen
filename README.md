ionic-ion-showWhen
==================
A set of utility directives for the Ionic Framework. ```showWhen``` and ```hideWhen``` act similar to the Ionic ```expose-aside-when``` attribute on the sidemenu that allows you to pass in a media query (or the word large which maps to a media query) that decides whether to show the side menu as a second column or behave as a side menu. This directive allows you to use that functionality on any element.

If the media query is true, the element will show. If it is not true, the element will be hidden.

Useful for tablet-only or phone-only content.

More Info: http://mcgivery.com/ionic-showwhen-directive/

A third directive is ```showWhenState``` which shows an element when the state name (or names) passed to and attribute match the current state.

##Usage

First, import the script into your page.

```
<script src="lib/ionic.ion.showwhen.js"
```

Next, import the module into your app.

```
angular.module('myCoolApp', ['ionic','ionic.ion.showWhen'])
```

Finally, mark an element with the attribute and a value.

```
<div show-when="large">test</div>
```

```
<div hide-when="large">test</div>
```

```
<div show-when-state="tabs.home">test</div>
```

```
<div show-when-state="tabs.about || tabs.facts">test</div>
```

Note: "large" maps to "(min-width:768px)"

Note: for ```show-when-state``` a || indicates OR logic.

##Questions
Feel free to ask any questions on twitter @andrewmcgivery
