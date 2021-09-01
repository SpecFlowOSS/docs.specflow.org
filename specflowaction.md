# SpecFlow Actions

SpecFlow Actions is our new way to help our users write easier and quicker test automation. We aim to solve common challenges you may encounter during your work of automating an application,API,website, and mobile app.

We do this for our community, therefore we want to work on actions that bring true value to you. Please go to our [SpecFlow Actions forum page](https://support.specflow.org/hc/en-us/community/topics/4404085862161-SpecFlow-Actions?sort_by=votes) and vote for your favorite action or suggest a new one.

There are two kinds of SpecFlow Actions:

- [Code snippets](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/CodeSnippets) - These are small code snippets that solve a particular problem.

- [Plugins](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins) To solve more complex problems, our team has put together a series of dedicated plugins for SpecFlow that provide more functionalities and integrate effortlessly into SpecFlow and its features.

## Code snippets

- [CSV](https://github.com/SpecFlowOSS/SpecFlow.Actions/blob/main/CodeSnippets/CSV.ipynb)

This code snippet allows you get the value of a cell using row and column name) from a .csv- file

- [Excel](https://github.com/SpecFlowOSS/SpecFlow.Actions/blob/main/CodeSnippets/Excel.ipynb)

Similar to the CSV code snippet this code allows you get the value of a cell using row and column name but from a .xlsx- file

- [Custom test output](https://github.com/SpecFlowOSS/SpecFlow.Actions/blob/main/CodeSnippets/TestOutput.ipynb)

This code snippets shows you how to bring your custom test output to the unit test runner of your choice. It supports NUnit, MSTest, xUnit and SpecFlow+ Runner.

----

## Plugins

- [Selenium](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins/SpecFlow.Actions.Selenium)

This plugin will help you use Selenium together with SpecFlow. It handles the lifetime of your browser and provides easy configuration and helper methods to interact with Selenium.

- [BoaConstrictor](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins/SpecFlow.Actions.BoaConstrictor)

This plugin will help you use [Boa-Constrictor](https://github.com/q2ebanking/boa-constrictor) together with SpecFlow to use the Screenplay Pattern for Selenium more easily.
In the background it is using [SpecFlow.Actions.Selenium](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins/SpecFlow.Actions.Selenium) so all functionality of it is also available, if you are using Boa-Constrictor.
Boa-Constrictor is configured out of the box. The logger is connected to the [SpecFlow Output API](https://docs.specflow.org/projects/specflow/en/latest/outputapi/outputapi.html).

- [Browserstack](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins/Specflow.Actions.Browserstack)

This plugin will help you use Browserstack and Selenium together with SpecFlow. As an extension of [SpecFlow.Actions.Selenium](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins/SpecFlow.Actions.Selenium), It handles the lifetime of your browser and provides seamless integration with the Browserstack Automate feature.

- [Docker](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins/SpecFlow.Actions.Docker)

This plugin will help you by using Docker together with SpecFlow.

- [Playwright](https://github.com/SpecFlowOSS/SpecFlow.Actions/tree/main/Plugins/SpecFlow.Actions.Playwright)

This plugin will help you use [Playwright](https://playwright.dev/) together with SpecFlow. It handles the initialization and lifetime of your browser, provides methods to work with your page selectors and a configuration that makes it easy to set up the browser instance.
