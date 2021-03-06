---
layout: page
title: Addons
---

# Addons

## Applications 

#### [WebCeption](https://github.com/jayhealey/Webception)

Webception is a deployable web-application that allows you to run all your Codeception tests in the browser.

You can access multiple test suites and decide which tests to include in a run. It allows you start, stop and restart the process whilst watching the test results in the Console.

## Modules

#### [CakePHP](https://github.com/cakephp/codeception)

Official CakePHP 3 module for Codeception.

#### [CakeCeption](https://github.com/hkzpjt/cakeception)

Integrate Codeception to CakePHP v2.* projects

#### [Date/Time](https://github.com/nathanmac/datetime-codeception-module)

This module provides additional helpers for your test to help with date and time comparisons.

#### [Doctrine1](https://github.com/Codeception/Doctrine1Module)

Module for Doctrine 1.x ORM (deprecated in Codeception 2.1)

#### [IM](https://github.com/nathanmac/im-codeception-module)

This module allows the testing against external messaging services as well as triggering notifications via your tests, currently supports HipChat messaging service.

#### [MailCatcher](https://github.com/captbaritone/codeception-mailcatcher-module) 

This module will let you test emails that are sent during your Codeception acceptance tests. It depends upon you having MailCatcher installed on your development server.

#### [MailTrap](https://github.com/WhatDaFox/Codeception-Mailtrap)

Codeception module to test email using Mailtrap.io

#### [Mockery](https://github.com/Codeception/MockeryModule)

Integrates Mockery into Codeception tests.

#### [Symfony1](https://github.com/Codeception/symfony1module)

Module for symfony 1.x framework (deprecated in Codeception 2.1)

#### [Remote File Attachment](https://github.com/phmLabs/codeception-module-attachfileremote)
This module helps to upload files when using webdriver via remote connection.

#### [VisualCeption](https://github.com/DigitalProducts/codeception-module-visualception)

Visual regression tests integrated in Codeception. This module can be used to compare the current representation of a website element with an expeted. It was written on the shoulders of codeception and integrates in a very easy way.

#### [WordPress Browser and Database](https://github.com/lucatume/wp-browser)

An extension of Codeception own PhpBrowser and Db modules to allow for easy and streamlined WordPress themes and plugins testing. 

## Extensions

Codeception extensions are developed by third-party contributors and can enhance test execution flow, by listening to internal events. [Read more about extensions](http://codeception.com/docs/08-Customization#Extension-classes).


### Official Extensions

Official Extensions are installed with Codeception but you should enable them manually. Also they are a good point to learn about developing your own extensions.

#### [Codeception\Platform\Logger](https://github.com/Codeception/Codeception/blob/2.0/src/Codeception/Platform/Logger.php)

Logs suites/tests/steps using Monolog library *(formerly enabled by default)*.

Enable it in `codeception.yml`:

{% highlight yaml %}
extensions:
    enabled: [Codeception\Platform\Logger]
{% endhighlight %}

#### [Codeception\Platform\RunFailed](https://github.com/Codeception/Codeception/blob/2.0/src/Codeception/Platform/RunFailed.php)

Saves failed tests into tests/_output/failed in order to rerun failed tests.

Enable it in `codeception.yml`:

{% highlight yaml %}
extensions:
    enabled: [Codeception\Platform\RunFailed]
{% endhighlight %}

Then you can run failed tests by running `failed` group:

```
codecept run -g failed
```

#### [Codeception\Platform\SimpleOutput](https://github.com/Codeception/Codeception/blob/2.0/src/Codeception/Platform/SimpleOutput.php)

Changes output style. If you need to implement your own output format you should use this extension as a starting point.

### 3rd Party Extensions

Extensions should be installed via **Composer**.

#### [Allure Codeception Adapter](https://github.com/allure-framework/allure-codeception)

This is a Codeception adapter for [Allure Framework](https://github.com/allure-framework).

#### [PhpBuiltinServer](https://github.com/tiger-seo/PhpBuiltinServer)

Extension for starting and stopping built-in PHP server. Works on Windows, Mac, Linux.

#### [Phantoman](https://github.com/site5/phantoman)

Extension for automatically starting and stopping PhantomJS when running tests.

#### [DrushDb](https://github.com/pfaocle/DrushDb)

DrushDb is a Codeception extension to populate and cleanup test **Drupal** sites during test runs using Drush aliases and the sql-sync command.

#### [Notifier](https://github.com/Codeception/Notifier)

Flexible notifications with [notificator](https://github.com/namshi/notificator) library. 

#### [RemoteDebug](https://github.com/tiger-seo/codeception-remotedebug)

Starts remote debug session during test execution.

#### [WPBrowser, WPDatabase, WPLoader](https://github.com/lucatume/wp-browser)

WordPress specific extensions of PHPBrowser and Db modules to allow for more streamlined testing of themes and plugins and a WordPress automated testing suite wrapper.

---

## IDE Plugins

#### [PHPStorm Command Line Tool](https://github.com/tiger-seo/codeception-phpstorm-commandlinetool)

Codeception CLI tool description for PhpStorm.



<div class="alert alert-warning">To publish your own extension <a href="https://github.com/Codeception/codeception.github.com/edit/master/addons.markdown">edit this page</a> on GitHub and submit a Pull Request. Please make sure you have installation guide and green light from Travis CI.</div>

