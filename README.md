# go-timer
[![license](http://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jeffjen/go-timer/master/LICENSE)
[![Build Status](https://travis-ci.org/jeffjen/go-timer.svg?branch=master)](https://travis-ci.org/jeffjen/go-timer)

A framework for handling time based resource management

## timer

Schedule work to run at specific time.  It uses implementation in
[container/heap](http://golang.org/pkg/container/heap/) to setup min-heap on
the TTL of the scheduled item.

## session

Based on timer, I present a simple in memory volaile KV storage inspired by
[redis](http://redis.io/).

Supported operations

- Set, Setexp
- Get
- Getset
- Expire
- TTL
- Del
- List, Listexp
- Watch
