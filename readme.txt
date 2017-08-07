=== Nosto - SaaS Recommendation Engine for WP e-Commerce ===
Contributors: nosto
Tags: nosto tagging, wp e-commerce, e-commerce, ecommerce, personalization, recommendation, recommendation engine
Requires at least: 3.5.0
Tested up to: 3.9.0
Stable tag: 1.0.3
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Nosto increases online store revenues by delivering customers a personalized shopping experience using behavioral data and real-time data processing.

== Description ==

Nosto’s risk free SaaS solution enables personalized product recommendations in real time. Its plug and play solution makes enterprise level recommendation engine easily accessible to a fraction of the typical cost to online stores of all sizes, automating marketing activities and increasing conversion, average order value, customer retention and store revenues as a result.

With Nosto’s WP e-Commerce extension implementation is quick and painless. Simply install the extension, add your own design for recommendations or use default themes provided and start improving your online sales. You can be up and running with personalized recommendations in less than an hour!

Display up- and cross-sell recommendations customizable with multiple rulesets to support your business goals.

Use personalized recommendations to target every individual visitor with product recommendations that particular visitor is most likely to buy, based on subsequential and trend data collected from your site.

Promote best converting products through top lists that update in real-time along with over thirty on-site recommendation features.

Send personalized triggered emails automatically to your customers. Nosto features multiple email types from abandoned cart email to customer retention campaigns.

Nosto is delivered directly from the cloud so it doesn’t increase your server load or slow down page load time.

Risk-free CPA, "no sales - no bill", pricing model and service delivered from cloud without contractual commitment.

START YOUR FREE TRIAL NOW! 

Install the extension, open up an account on www.nosto.com, choose WP e-Commerce as your platform in the sign-up and start your 14 day free trial today - no credit card required!

== Installation ==

Before proceeding please make sure that you are running WordPress 3.5 or above and WP e-Commerce 3.8.9.1 or above.

Please refer to the WordPress documentation on how to get the plugin to appear in your installation admin section.

Once the plugin appears in your installation, you must activate it. Navigate to the "Plugins" section and locate the
"WP e-Commerce Nosto Tagging" plugin. The activation is done simply by clicking the "Activate" link next to the plugin
name in the list.

The activation procedure will create a new page called "Top Sellers". This page can be found and edited under the
"Pages" section in the backend. The page contains a single div element that is used to show product recommendations. A
link to the page should appear in the shops main navigation menu.

The plugin uses the WordPress Action API to add content to the shop. However, there are a few actions that will have to
be added to the shops theme in order for the plugin to function to its full extent.

* wpecnt_top_of_search_results
	* This action should be called above the search result list on the on search pages
	* You need to add `<?php do_action('wpecnt_top_of_search_results'); ?>` in your themes search page template at the
	appropriate location
* wpecnt_bottom_of_search_results
	* This action should be called below the search result list on the on search pages
	* You need to add `<?php do_action('wpecnt_bottom_of_search_results'); ?>` in your themes search page template at
	the appropriate location
* wpecnt_top_of_pages
	* This action should be called at the beginning of every page in the shop
	* You need to add `<?php do_action('wpecnt_top_of_pages'); ?>` in your themes header template, inside the main
	content section
* wpecnt_bottom_of_pages
	* This action should be called at the end of every page in the shop
	* You need to add `<?php do_action('wpecnt_bottom_of_pages'); ?>` in your themes footer template, inside the main
	content section

Once you have activated the plugin and added the necessary actions, you need to configure the plugin. The plugins
configuration page can be found under the "Settings->Store" section, in the tab called "Nosto Tagging".

The configuration page consists of three settings:

* Server address
	* This is the server address for the Nosto marketing automation service
	* It will have the default value of "connect.nosto.com" and you do not need to change this
* Account name
	* This is your Nosto marketing automation service account name that you got when registering for the service
* Use default Nosto elements
	* This setting controls if the plugin should create and output the default Nosto elements for showing the product
	recommendations
	* You can disable the defaults if you want to use your own elements in your theme

All of the above settings are needed for the plugin to work.

The "Nosto Tagging" widget added by the plugin for showing Nosto elements in the shops sidebars, needs to be configured
if you wish to use it. The widget can be found under the "Appearance->Widgets" section and it works like any other
WordPress widget. After dropping the widget in the appropriate sidebar container, you need to configure its Nosto ID.
This ID is used as the Nosto element div ID attribute and can be whatever you decide.

== Changelog ==

= 1.0.3 =
* Change recommendation element naming policy

= 1.0.2 =
* Add own method to find lowest product variation price

= 1.0.1 =
* Hide "Server address" from plugin configuration
* Change "Account name" to "Account ID" in plugin configuration
* Remove html escape from product description in product tagging
* Change order tagging buyer info to always come from the checkout form billing address
* Update embed script

= 1.0.0 =
* Initial release

== Screenshots ==

1. Get a real-time view of what visitors are doing on your site and start learning more about their behavior and preferences.
2. Nosto Recommendations as seen on www.joythestore.com.
