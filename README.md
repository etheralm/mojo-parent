# MojoHaus Parent

This is the parent pom for all [MojoHaus](http://www.mojohaus.org) Maven plugins and components.
 
[![Build Status](https://travis-ci.org/mojohaus/mojo-parent.svg?branch=master)](https://travis-ci.org/mojohaus/mojo-parent)

## Releasing

* Make sure `gpg-agent` is running.
* Execute `mvn -B release:prepare release:perform`

For publishing the site, do the following (assuming mono-module project):

```
cd target/checkout
mvn -Preporting verify site-deploy
```
