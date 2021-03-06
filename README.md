cherami-thrift 
==============
[Cherami](https://eng.uber.com/cherami/) is a distributed, scalable, durable, and highly available message queue system we developed at Uber Engineering to transport asynchronous tasks. 

This repo holds thrift IDL files and generated code used by Cherami to communicate between server and clients, or between components within Cherami. This repo is not end-user useful on its own, but needed only when a feature require IDL changes. If you are a developer looking to use Cherami, please instead use [`cherami-client-go`](https://github.com/uber/cherami-client-go) repo and [`cherami-server`](https://github.com/uber/cherami-server) repo.


Developing
----------
The `cherami-thrift.git branch specifically holds the thrift definition along with the autogenerated code for the thrift APIs.

Prerequisite:
* Make certain that `thrift` is in your path. (OSX: `brew install thrift`) 
* `thrift-gen` is needed (`go get github.com/uber/tchannel-go/thrift/thrift-gen`)

After editing the thrift files, run `make bins` to generate code:

Contributing
------------
We'd love your help in making Cherami great. If you need new API(s) to be added to our thrift files, open an issue and we will respond as fast as we can. If you want to propose new feature(s) along with the appropriate APIs yourself, open a pull request to start a discussion and we will merge it after review.

**Note:** All contributors also need to fill out the [Uber Contributor License Agreement](http://t.uber.com/cla) before we can merge in any of your changes

Documentation
--------------
Interested in learning more about Cherami? Read the blog post:
[eng.uber.com/cherami](https://eng.uber.com/cherami/)

License
-------
MIT License, please see [LICENSE](https://github.com/uber/cherami-thrift/blob/master/LICENSE) for details.
