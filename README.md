[![Build Status](https://travis-ci.org/grails-plugins/grails-platform-core.svg)](https://travis-ci.org/grails-plugins/grails-platform-core)

# Grails Plugin Platform -> Upgraded to Grails 3.2.4+ and Java 8

I'm currently having issues with 

compile 'org.grails.plugins:platform-core:1.0.0'


runtime 'org.grails.plugins:platform-core:1.0.0'

The platform-core code loads during compile and dependency reporting. 

However, the objects inside of the platform-core can't be loaded by compile.

# Grails Plugin Platform for Grails 3.2.4+ and Java 1.8

This plugin provides a suite of facilities to support the plugin ecosystem by
providing the mechanisms for plugins to play nicely with each other and the
developer's app.

This is intended to stay out of the Grails versioning cycle as much as
possible, to provide support for these features across Grails releases as much
as possible

See the [documentation](http://grailsrocks.github.com/grails-platform-core/guide/) for more details.
