# Worldpay Within - The Java SDK

The Java implementation for the Worldpay Within IoT payment SDK. This SDK, or Software Development Kit, enables smart devices to discover each other, negogiate a price for services, make a payment (through the Worldpay payments gateway) for services, and then consume services via a 'trusted trigger'. For more information see our documentation website here: http://www.worldpaywithin.com

![The Worldpay Within puzzle piece](http://wptechinnovation.github.io/worldpay-within-sdk/images/architecture/worldpayWithinFig1.png)

## Get started
1. Download this repo
2. Add the example projects to netbeans (or go it alone creating your own project from the source code and jars - In your project, reference `WPWithin.jar` from the releases section and the other jars in lib)
3. Run the examples...

## Run the examples
* Run the consumer project
* Simultaneously run the producer or producer-callbacks project
* The two smart devices should communicate with each other and make a payment

## Compatibility and pre-requisites
* Assumption here is you have the Java 1.8 JRE at least
* Java 1.8 SDK even better

## See the payments:
1. Sign up to https://online.worldpay.com if you haven't already done so
2. Got to settings > API keys and get your test keys
3. Replace the keys in the consumer and producer java example source files
4. Re-run the examples and you should see the payments coming through on the WPOP (Worldpay Online) payments dashboard

## Debugging:
* If you get some odd error messages talking about a 'rpc-agent'
* Try typing the following command: 'ps -e | grep rpc' to get the pid(s) of rpc-agents that are running. 
* Then do kill &lt;pid&gt; e.g. kill 13249234 to kill these processes.
* Try re-running the examples - if this fails then please contact us at innovation@worldpay.com or on our slack channel or raise an issue in github.
  
## So what does it do:

![The Worldpay Within Flows sequence diagram](http://wptechinnovation.github.io/worldpay-within-sdk/images/architecture/serviceOverview.png)

You can see there are four phases; discover, negotiation, payment and then service delivery, for more information visit our website at http://www.worldpaywithin.com.

[The flows and API can be found here](http://wptechinnovation.github.io/worldpay-within-sdk/the-flows.html)

## The Javadoc

[The javadoc for the wrapper can be found here](http://wptechinnovation.github.io/worldpay-within-sdk/wrapper-doc/javadoc/)

## Want to contribute:

Want to contribute, then please clone the repo and create a branch, once you've made your changes create a pull request, we will review your code, and if accepted it will be merged into the code base. You can also raise issues here on github, or contact us direct at innovation@worldpay.com or alternatively join our slack channel at iotpay.slack.com.
