# install latest package

I prefer to run Snap as a service, so we will first prep for pulling from Package Cloud:  

`
$ cd ~
$ curl -s https://packagecloud.io/install/repositories/intelsdi-x/snap/script.deb.sh | sudo bash
`

And now we can install the package: 

`
$ apt-get install snap-telemetry
`

It's important to note that these packages are **available for testing purposes**. We strongly recommend signing any binaries you plan to run in production. Read more about these [security considerations here](https://github.com/intelsdi-x/snap/blob/master/docs/PLUGIN_SIGNING.md).

// Note to self - need to point toward docs on production preparation.. not just plugin signing.