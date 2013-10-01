# Installation

Lemur Learning is an app built on top of the [Elefant CMS](http://www.elefantcms.com/download) platform.
Follow the steps on the Elefant website to get the base CMS up and running,
then follow these steps to install Lemur Learning:

1\. From the root folder of the site, run the following command:

	php composer.phar require elefant/app-lemur

This will also install the following apps that Lemur depends on:

* [Comments](https://github.com/jbroadway/comments)
* [SCORM](https://github.com/jbroadway/scorm)
* [Stripe Payments](https://github.com/jbroadway/stripe)

> **Note:** You may need to add `"minimum-stability": "dev"` to your `composer.json`
> file in order for Composer to work correctly while Lemur is still in development.

> **Payments:** Additional payment providers can be supported by implementing the
> [payment handler interface found here](https://github.com/jbroadway/stripe#creating-a-member-payment-or-subscription-form).
> More documentation and examples still to come.

2\. Copy the file `apps/lemur/sample_bootstrap.php` into your document root and rename
it `bootstrap.php`. If a `bootstrap.php` already exists, open the file and add the
relevant lines of code to your existing `bootstrap.php` file.

	cp apps/lemur/sample_bootstrap.php bootstrap.php

3\. Copy the `apps/lemur/theme` folder into your `layouts` folder and rename it `lemur`.

	cp -R apps/lemur/theme layouts/lemur

4\. Log into Elefant and run the Lemur installer by navigating to Tools > Courses.

### Optional steps

5\. Go to Tools > Navigation and add the `Courses` page to your site tree.

6\. Go to Tools > Designer and set the Lemur layout as your default.

7\. Copy the `product.php` file from your `apps/lemur` folder into the global
`conf` folder, overwriting the existing copy. This will replace the Elefant
branding with Lemur's own.

	cp apps/lemur/product.php conf/product.php

You should now have a working Lemur Learning installation.

Next: [[:Support]]