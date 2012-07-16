nodeunit-watcher
========

A wrapper for [nodeunit](https://github.com/caolan/nodeunit/) to provide continuous testing.

Usage
-----

nodeunit-watcher is simply a wrapper around your existing version of nodeunit.  Instead of calling `nodeunit` to execute tests, you execute `nodeunit-watcher` with your desired nodeunit options like so:

    nodeunit-watcher --reporter minimal testfile.js
    
nodeunit-watcher checks your test files and calls `fs.watchFile` on them and calls a new instance of `nodeunit` whenever you make changes to the file specified.

Bug Reports
-----

https://github.com/AlexCline/nodeunit-watcher/issues