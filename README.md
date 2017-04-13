# \<isw-route\>

Router with app-route like API, wrapped in an iron-selectable element that binds the active route.

Demo Link: https://www.webcomponents.org/element/IswPolymerElements/isw-route/demo/demo/index.html

```html
<app-location route="{{route}}"></app-location>

<isw-route-selector route="[[route]]" attr-for-selected="route" selected="{{selectedRoute}}" data="{{data}}">
  <isw-route route="a" pattern="/route-a"></isw-route>
  <isw-route route="a" pattern="/route-a/route-b"></isw-route>
  <isw-route route="a" pattern="/route-c/:somedata"></isw-route>
  <isw-route route="a" pattern="/route-c/route-d"></isw-route>
</isw-route-selector>

<iron-pages attr-for-selected="route" selected="[[selectedRoute]]">
  <div route="a">Route A</div>
  <div route="b">Route B</div>
  <div route="c">Route C</div>
  <div route="d">Route D</div>
</iron-pages>
```