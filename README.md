﻿# Braintree ASP.NET Example
An example Braintree integration for ASP.NET

## Setup Instructions
These instructions assume you are using Visual Studio Professional 2013. This has not been tested in Xamarin Studio, or other versions of Visual Studio. This project is also set up
to use NuGet package restore, so all dependencies should be automatically installed.

1. Open `braintree_aspnet_example.sln` in Visual Studio

2. Open the `Web.config` in `BraintreeASPExample`, and fill in your Braintree API Credentials in the `BraintreeEnvironment`, `BraintreeMerchantId`, `BraintreePublicKey`, and `BraintreePrivateKey` keys.
   Credentials can be found by navigating to Account > My user > View API Keys in the Braintree control panel. Full instructions can be [found on our support site](https://articles.braintreepayments.com/control-panel/important-gateway-credentials#api-credentials).

3. Start the project by pressing the play button in the toolbar.

## Running Tests

There are unit and integration tests. To run the integration tests, you will need to have IIS Express and Firefox installed and your API credentials filled in. You can run all the tests by opening the Test Explorer and clicking `Run All`.

## Pro Tips

 * If you do not want to or are unable to use NuGet package restore, make sure to download and reference the following packages:
   * [Braintree](https://developers.braintreepayments.com/start/hello-server/dotnet#install-and-configure) 2.53.0 or higher
   * [Moq](https://github.com/Moq/moq4) 4.2 or higher (needed for `BraintreeASPExampleTests` only)
   * [Selenium WebDriver](https://www.seleniumhq.org/download) 2.52 or higher (needed for `BraintreeASPExampleTests` only)

## Disclaimer

This code is provided as is and is only intended to be used for illustration purposes. This code is not production-ready and is not meant to be used in a production environment. This repository is to be used as a tool to help merchants learn how to integrate with Braintree. Any use of this repository or any of its code in a production environment is highly discouraged.

