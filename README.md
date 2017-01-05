[![Build Status](https://travis-ci.org/grails-plugins/grails-platform-core.svg)](https://travis-ci.org/grails-plugins/grails-platform-core)

# NON-WORKING AT THIS POINT

# Grails Plugin Platform -> Upgrade to Grails 3.2.4+ and Java 8

I'm currently having issues with 

compile 'org.grails.plugins:platform-core:1.0.0'


runtime 'org.grails.plugins:platform-core:1.0.0'

The platform-core code loads during compile and dependency reporting. 

However, the objects inside of the platform-core can't be loaded by compile.

# Theory

I'm thinking there is a name collision between grails 3.2.4 and it's libraries 
with platform-core plugin. Specifically in the area of Events. Specifically shows itself error below.

102: unable to resolve class grails.events.Listener ,  unable to find class for annotation
 @ line 102, column 2.
        @grails.events.Listener(topic = "accountCacheDelete", namespace = "<project_namespace>")
    ^

# Grails Plugin Platform 

This plugin provides a suite of facilities to support the plugin ecosystem by
providing the mechanisms for plugins to play nicely with each other and the
developer's app.

This is intended to stay out of the Grails versioning cycle as much as
possible, to provide support for these features across Grails releases as much
as possible

See the [documentation](http://grailsrocks.github.com/grails-platform-core/guide/) for more details.
