Packaging [onboard.js](https://github.com/nozzle/onboard.js) for [Meteor.js](http://meteor.com).


# Meteor

If you're new to Meteor, here's what the excitement is all about -
[watch the first two minutes](https://www.youtube.com/watch?v=fsi0aJ9yr2o); you'll be hooked by 1:28.

That screencast is from 2012. In the meantime, Meteor has become a mature JavaScript-everywhere web
development framework. Read more at [Why Meteor](http://www.meteorpedia.com/read/Why_Meteor).

To install the package, simply run

```bash
$ meteor add 416serg:onboard
```

## Using

In you template, first attach the onboard to the body or other wrapping element you'd like to mask:

```HTML
var onboard = $("body").onboard();
```

Then attach the steps to the elements to highlight, using jquery selectors:

```HTML
onboard.addStep("#hello", "This step says hello");
onboard.addStep("#world", "This step says world");
```

Or instantiate onboard with predefined steps:

```HTML
var onboard = $("body").onboard({
  steps: [{
    selector: '#element1',
    introduction: 'This is the first element'
  },{
    selector: '#element2',
    introduction: 'This is the second element'
  },{
    ....
  }]
});
```

Then start the show!

```HTML
onboard.start();
```

# Issues

If you encounter an issue while using this package, please CC @416serg when you file it in this repo.


# TODO

* Tests
* Tests ensuring correct event handling on template re-rendering
