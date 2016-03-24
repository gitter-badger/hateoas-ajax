# hateoas-ajax [![Build Status](https://travis-ci.org/Nemo64/hateoas-ajax.svg?branch=master)](https://travis-ci.org/Nemo64/hateoas-ajax)

[![Join the chat at https://gitter.im/Nemo64/hateoas-ajax](https://badges.gitter.im/Nemo64/hateoas-ajax.svg)](https://gitter.im/Nemo64/hateoas-ajax?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

An extension of polymer's [`iron-ajax`](https://elements.polymer-project.org/elements/iron-ajax)
but with an addition of some magic related to [hateoas](http://en.wikipedia.org/wiki/HATEOAS).

## setup

```HTML
<!-- replace core-ajax with hateoas-ajax -->
<hateoas-ajax url="{{url}}" response="{{response}}"></hateoas-ajax>
```

## perform get

```JSON
{
  "name": "Max",
  "_links": {
    "address": {
      "href": "[request url]"
    }
  }
}
```

```HTML
<!-- simply call relations like they are properties -->
<!-- they are requested and though data binding automatically displayed when present -->
<div>{{person.address}}</div>
```

## Documentation
[component page](http://Nemo64.github.io/hateoas-ajax/)
