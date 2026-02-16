# loopSubscription-customBundle-widget
Loop Subscription Integrated Custom Widget for Bundle Purchase

This project is a custom Shopify section built to integrate with the Loop Subscription App and create a smooth bundle-style subscription experience.

## The goal was simple:
Make it easy for customers to select subscription-based products from a collection, view pricing clearly (including discounts), choose delivery frequency, adjust quantity, and add everything to the cart in a clean and user-friendly way.

Instead of using a default subscription layout, this widget gives more control over UI, pricing display, and cart behavior.


## What This Widget Does

- Displays products dynamically from a selected Shopify collection
- Automatically detects and attaches the correct selling plan
- Shows subscription price and compare-at price
- Calculates and displays discount percentage
- Allows customers to switch between subscription and one-time purchase
- Includes quantity selector
- Adds items to cart using Shopify AJAX API
- Automatically opens cart drawer after adding to cart

## Built With

- Shopify Liquid
- Vanilla JavaScript
- Shopify AJAX Cart API
- Shopify Selling Plan API
- Loop Subscription App

## How It Works (Simple Flow)

- The merchant selects a collection inside the section settings.
- All products from that collection are displayed inside the custom widget.
- The first product is auto-selected by default.

### When a product is selected:

- Variant ID is captured
- Selling Plan ID is detected
- Price and discount are updated dynamically

### When “Add to Cart” is clicked:

- Product is added with selling plan (if subscription selected)
- Custom properties are attached
- Page reloads (if needed)
- Cart drawer opens automatically

## Why I Built It
The default subscription layouts often don’t allow flexibility when showing multiple products together under a unified experience.

### This widget was built to:

- Provide better UI control
- Improve customer clarity around pricing
- Support bundle-style subscription purchasing
- Maintain compatibility with Shopify’s cart system

## Installation Steps

- Go to Shopify Admin
- Online Store → Themes
- Click "Edit Code"
- Create a new Section file
- Paste the widget code
- Add the section to your page
- Select the subscription products collection
