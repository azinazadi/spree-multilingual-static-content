SpreeMultilingualStaticContent
==============================
[Spree Static Content](http://google.com), is a Good, clean content management of pages for Spree, but it is not possible 
to have the pages in different languages, like other spree features.

using this extension you will have your pages in multiple languages also. it uses the standard spree_i18n methods.

Installation
------------

Add spree_multilingual_static_content to your Gemfile. You need to have spree_static_content also. spree_static_content extension is an addition to spree_static_content and make that multilingual.


```ruby

gem 'spree_static_content', github: 'spree/spree_static_content', branch: 'master'
gem 'spree_multilingual_static_content', :github => "azinazadi/spree-multilingual-static-content"

```



Bundle your dependencies and run the installation generator:

```shell
bundle
bundle exec rails g spree_multilingual_static_content:install
```

it is compatible with spree 2.1, and will work also with older versions...
Testing
-------

Be sure to bundle your dependencies and then create a dummy test app for the specs to run against.

```shell
bundle
bundle exec rake test_app
bundle exec rspec spec
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_multilingual_static_content/factories'
```

Copyright (c) 2013 [Azin Azadi], released under the New BSD License
