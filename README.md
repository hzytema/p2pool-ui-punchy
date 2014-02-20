p2pool-node-status
==================

An alternative clean p2pool node dashboard. It uses Bootstrap, jQuery and Highcharts.

## Installation

To run this dashboard in parallel to your current p2pool web interface, do in your web-static directory:

```
git clone https://github.com/johndoe75/p2pool-node-status.git
```

If you want to use it as replacement for your current web-static, then do in the top directory of your p2pool installation

```
mv web-static _web-static-pre
git clone https://github.com/johndoe75/p2pool-node-status.git web-static
```

### Use a different host

You can run this interface on a different host than your p2pool node.  To do so you need to configure the API address of your p2pool server.  For this set the variable `host` in index.html appropriately.  E.g.:

```
var host= 'http://p2pool.org:9332';
```

In order to run this UI like this, the node the UI is running on must have PHP available.  This is required due to a required JSONP handler.

Beware:  This will put network traffic on your p2pool node just for periodically fetching stats from p2pool API!  It can, but must not, result in a higher variance!

### Highlight your own miner address

If you want your miner address highlighted, adjust `myself` variable accordingly. E. g.

``` JavaScript
var myself= [
  '1MzFr1eKzLEC1tuoZ7URMB7WWBMgHKimKe'
];
```

…

## Credits & License

Alexander Zschach <alex@zschach.net>

### Donate

If you like this tool, find it useful or if you just find it useful, that people out there writing free software for everybody to use or contribute, please donate some coins:

Bitcoins 1MzFr1eKzLEC1tuoZ7URMB7WWBMgHKimKe  
Litecoins LSRfZJf75MtwzrbAUfQgqzdK4hHpY4oMW3  
Terracoins 1MsuC6knLeZKHCyQ39Xcw1qcgScS1ZK5R  
Feathercoins 6tfEE48qk8Kgs9ancC82Y2iQBSX3VGYXfL

### License

The MIT License (MIT)

Copyright (c) 2013 Alexander Zschach alex@zschach.net

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

--------------------------

:wq!

