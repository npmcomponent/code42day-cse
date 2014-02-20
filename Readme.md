*This repository is a mirror of the [component](http://component.io) module [code42day/cse](http://github.com/code42day/cse). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/code42day-cse`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# cse

Use Google [custom search engine][cse] on your page.

See in the wild on the [American Scenic Byways][byways.site] website - _[source][byways.src]_.

## Installation

Install with [component(1)](http://component.io):

    $ component install code42day/cse

## API

You need to create [custom search engine][cse] and obtain search engine ID whithc looks like this:
`012345678901234567890:abcdefghijk`


Add `#cseSearchBox` or `#cseSearchResults` (or both) to your HTML and then initialize them with
google's magic.

````javascript
var cseID = "012345678901234567890:abcdefghijk";
require('cse')(cseID);
````

If neither `#cseSearchBox` nor `#cseSearchResults` are found we die silently without trying to load
any scripts from google.


## License

  MIT

[cse]: http://google.com/cse
[byways.site]: http://scenicbyways.info/search.html?q=ground
[byways.src]: https://github.com/code42day/byways