# Gravity Forms + Stripe
http://wordpress.org/extend/plugins/gravity-forms-stripe/

[Stripe](https://stripe.com) allows you to process credit cards directly on your site, securely and easily, without having to deal with merchant accounts, PCI-compliance, or PayPal.

This [Gravity Forms](http://naomicbush.com/getgravityforms) add-on integrates Stripe with your forms (adapted from the Gravity Forms Authorize.net Add-On) using the provided [Stripe.js](https://stripe.com/docs/stripe.js) to make sure sensitive card information never hits your server.

## Supporters
[deckerweb](https://github.com/deckerweb), [admodiggity](https://github.com/admodiggity), [pnommensen](https://github.com/pnommensen), [Linda C.](http://askmepc.com/), [jacobdubail](https://github.com/jacobdubail), [Michael S.](http://markandphil.com/), [Mark C.](http://bizelevator.com/), [willshouse](http://profiles.wordpress.org/willshouse), Dan B., Aaron A., [wpcdn](http://profiles.wordpress.org/wpcdn), [feshin](http://profiles.wordpress.org/feshin), Scot R., Teresa O.

## Features
* This plugin does one thing and one thing well: One-time payments
* with hooks to extend the plugin and add in your own functionality

## Want [more Stripe](http://gravityplus.pro)?
* Recurring payments/subscriptions
* Coupons
* Invoice line items
* Stripe + PayPal option on same form
* Pretty receipts?

[Get More Stripe here](http://gravityplus.pro)

## Requirements
* WordPress 3.4.2
* PHP 5.3 (although it worked for me when initially tested on 5.2 server)
* Gravity Forms 1.6.9 - [Grab a license](http://naomicbush.com/getgravityforms "purchase Gravity Forms!") if you don't already have one
* [Stripe](https://stripe.com) account

## Support
* Do NOT contact Gravity Forms OR Stripe for help with this add-on. They do not provide support for this plugin.
* Full support is available at [gravity+](http://gravityplus.pro)
* Support is not provided for free or via the WordPress forums, but feel free to help one another.

## Current Limitations
* Cannot have Stripe Add-On "activated" at the same time as Authorize.Net or PayPal Pro Add-Ons
* For security reasons, credit card field has to be on the last page of a multi-page form
* Can only setup 1 Stripe feed per form

## Known Conflicts

* Shortcodes Ultimate
* poorly coded Themeforest themes

## Installation

1. Upload `gravityforms-stripe` to the `/wp-content/plugins/` directory
2. Make sure that Gravity Forms is activated
3. Activate the plugin through the 'Plugins' menu in WordPress
4. Add your Stripe API keys to the Stripe tab on the Settings page (Forms->Settings).
5. Create a form, adding at least one product field along with the new 'Credit Card' field that appears under 'Pricing Fields.' Keep in mind that Stripe accepts a minimum charge of $0.50 - this means that the total amount of your form must be at least $0.50.
6. Under Forms->Stripe, add a Stripe feed for your new form.

## Changelog
### 1.6.9.1 (November 1, 2012)
* Switch to new version scheme that follows Gravity Forms
* Create a customer in Stripe for all transactions
* Fix Stripe JS to work without AJAX
* Fix issue with plugin not deactivating on uninstall
* Update to work with new Gravity Forms 1.6 fields
* Remove deprecated Stripe token parameter
* Allow unactivated Stripe test accounts to use in Test mode only

### 0.1.3 (April 19, 2012)
* Fix credit card field conflict with other GF payment add-ons
* Load Stripe JS only when form with a credit card field *and* Stripe feed is loaded
* Fix removal of credit card expiration date from information sent to server
* Add validation check for cardholder name and address
* Don't process payment if total is less than $0.50

### 0.1.2
* Fix error handling

### 0.1.1
* Fix "Class 'Stripe' Not Found" error

### 0.1 (April 3, 2012)
* First release

## License
This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program; if not, write to:

Free Software Foundation, Inc. 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.