New Relic Agent
================

A Cordova / PhoneGap plugin to add the New Relic Mobile Agent to your application. 

__NOTE:__ This plugin requires Cordova / PhoneGap >= 3.3.0 in order to support installation and linking of custom frameworks.

Installation
===============

`cordova plugin install http://github.com/crooy/newrelic-cordova`

__NOTE:__ There is currently an [issue](https://issues.apache.org/jira/browse/CB-6092) with publishing plugins that have frameworks with symlinks. Please install using the url rather than just the identifier.

you need to add the class rewrite to you ant options like so:
`export ANT_OPTS="-javaagent:/path/to/newrelic-android-4.120.0/lib/class.rewriter.jar"`

Configuration
===============

Get your mobile app's token from the New Relic portal and add it to your `config.xml` like so:

`<preference name="NewRelicApplicationToken" value="YOUR_TOKEN_HERE" />`

License
==============

The code for this plugin is covered under the Apache 2 License. See the [license file](LICENSE).

__NOTE:__ This license only applies to the *plugin code*. Please see the [New Relic license file](src/ios/NewRelicFramework/LICENSE) for the license that applies to the New Relic framework code.
