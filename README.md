# tag-entity-buttons

A Polymer Element showing positive and negative buttons to classify tags.

### Example
```js
var tags = {
  tag1: {
    database: '',
    type: 'ad',
    user: ''
  },
  tag2: {
    database: 'positive',
    type: 'ad',
    user: ''
  }
};
```

```html
<tag-manager tag-manager="{{tagManager}}"></tag-manager>
<tag-entity-buttons
  tag-manager="[[tagManager]]"
  tags="[[tags]]">
</tag-entity-buttons>
```

### Styling

`<tag-entity-buttons>` provides the following custom properties and mixins for styling:

Custom property        | Description                     | Default
-----------------------|---------------------------------|--------
`--tag-color`          | The color of the default tags.  | paper-grey-600
`--tag-negative-color` | The color of the negative tags. | paper-red-600
`--tag-positive-color` | The color of the positive tags. | paper-green-600
### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

