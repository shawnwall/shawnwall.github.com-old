---
layout: post
title: "FSNetworking: A Small Networking Library for iOS and Mac"
date: 2012-07-20 14:16
comments: true
categories: 
---

A few days after I finally put together my iOS third-party library [list](/ios/libraries.html), it's
time to add another great component for simplified networking -
[FSNetworking](https://github.com/foursquare/FSNetworking) from the folks at
[foursquare](http://engineering.foursquare.com/2012/07/19/say-hello-to-fsnetworking-a-small-networking-library-for-ios-and-mac/). A quick peek at the source reveals a grand total of two classes - FSNConnection & FSNData along with some categories which makes FSNetworking one of the most simplified networking libs I've seen yet. 

It's a block-based API which is a must-have for networking these days. Within a
single call you can set a parseBlock, completionBlock and a progressBlock for
callbacks. Example code is included for both iOS & Mac. 

At a quick glance it's missing the wonderful
[AFHTTPClient](https://github.com/AFNetworking/AFNetworking/blob/master/AFNetworking/AFHTTPClient.h) singleton pattern
found in [AFNetworking](https://github.com/AFNetworking/AFNetworking) although in their own example they show they use a FSAPI
singleton so it would be nice for them to create a pattern for us to follow
there. 

