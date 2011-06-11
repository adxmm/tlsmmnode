You need to require node.js for using this script. Node.js is super fast and it can convert super big file.

approximate long time is 1 MB = 1.3 seconds

But it's base on zawgyi text.

How to use
----------

	$ node index.js zawgyi.txt

and you will get output file in **output.txt** , same folder of index.js

Credit
------

tlsmmnode.js is copy from [MyanmarConverter.xpi](http://www.thanlwinsoft.org/MyanmarConverter/ "MyanmarConverter"). I just add following line in lines 1493

	exports.convert=function tlsConvert(input_val)
        {
            //var debug = new TlsDebug();
            var converter = tlsMyanmarConverters["zawgyi-one"];
            return converter.convertToUnicode(input_val);
        };