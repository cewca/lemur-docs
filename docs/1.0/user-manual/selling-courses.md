# Selling courses

## Prerequisites

First, you will need a [Stripe Payments](https://stripe.com/) account to handle the
payment processing.

You will also need an SSL certificate for your web server so it can accept secure
HTTPS connections.

Here are some places to buy an SSL certificate:

* [StartSSL](https://www.startssl.com/?app=1) - Free and paid
* [GoGetSSL](https://www.gogetssl.com/) - Paid
* [DNSimple](https://dnsimple.com) - Paid
* [Gandi.net](http://www.gandi.net/) - Paid

And here are some instructions for installing an SSL certificate on your web server:

* [Nginx web server](http://wiki.nginx.org/HttpSslModule)
* [Apache web server](http://httpd.apache.org/docs/2.2/ssl/ssl_howto.html)

## Configuration

To setup your site for selling courses, log in and go to Tools > Strip Payments > Settings.
Enter the secret key and publishable key from your [Stripe account area](https://manage.stripe.com/account/apikeys).
You can also change the currency to use for your site on this screen if necessary.

You can leave the `Custom handlers` and `Subscription plans` sections as they are, as these
are not needed for selling courses in Lemur.

Next, go to Tools > Courses > Settings and select `Stripe Payments` in the `Payment handler`
field and save your settings.

## Setting your price

You can set the price for a course in the `Add Course` form or by clicking on the `Settings`
link for an existing course.

In the course settings, first set the `Availability` to `Public - Paid`. This means that
the course should be publicly visible but sits behind a paywall. You'll notice that when
this setting is set, a `Price` field appears below it.

Set your price in the price field, using a decimal point to specify cents if you need, then
click the `Save Course` button to save your changes.

Visitors to the course listing page on your site should now see the course description along
with a button that says `Join this course - $24.99`.

## Other payment providers

Lemur currently only supports [Stripe](https://stripe.com/) as a payment provider. Additional
providers will be supported in the future, but for now Stripe is an excellent payment
processor that supports a growing list of countries.

[See here](https://github.com/jbroadway/stripe/wiki/Writing-custom-payment-providers)
for more information on implementing custom payment providers for the Elefant CMS framework.

Next: [[Administration]]