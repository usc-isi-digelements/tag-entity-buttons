# tag-entity-buttons

A Polymer Element showing buttons to classify an entity as either positive or negative for one or more tags.

### Example
```js
var classification1 = {
  database: '',
  type: 'ad',
  user: ''
};

var classification2 = {
  database: 'positive',
  type: 'ad',
  user: ''
};

var classification3 = {
  database: 'negative',
  type: 'ad',
  user: ''
};

var tags = {
  tag1: classification1,
  tag2: classification2,
  tag3: classification3
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

Custom property                     | Description                                       | Default
------------------------------------|---------------------------------------------------|--------
`--tag-button-color`                | The color of the untagged buttons.                | paper-grey-600
`--tag-button-negative-color`       | The color of the negatively tagged buttons.       | paper-red-600
`--tag-button-negative-hover-color` | The hover color of the negatively tagged buttons. | paper-red-900
`--tag-button-positive-color`       | The color of the positively tagged buttons.       | paper-green-600
`--tag-button-positive-hover-color` | The hover color of the positively tagged buttons. | paper-green-900

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

