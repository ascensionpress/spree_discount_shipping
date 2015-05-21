SpreeDiscountShipping
=============

Apply discounts to shipping methods in Spree Commerce.

### Features

* Easily set shipping discounts on new and existing shipping methods through the Spree admin GUI.
* Shipping amounts are calculated with: `calculator_cost * (100 - discount)/100.0`. This can be adjusted [here](#).
* Easily set default shipping discounts that apply to all shipping methods.
* View shipping discounts from the shipping_methods index.
* All existing shipping methods default to a 0% discount.
* No modifications to any of your `Spree::Calculator` classes are required--even if those classes are custom.


Installation
=======

Add the following line to your `Gemfile`:

```ruby
gem 'spree_discount_shipping', github: 'davidlaprade/spree_discount_shipping', branch: '1-3-stable'
```

Then:
```shell
bundle install
```

Then:
```ruby
bundle exec rails g spree_discount_shipping:install
```

Annnnnd you're done!

After installation, a new field ("Discount %") will be available to set through the Spree Admin GUI from `/admin/shipping_methods/new`.

Copyright (c) 2015 David Laprade, released under the New BSD License
