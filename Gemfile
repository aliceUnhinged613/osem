# frozen_string_literal: true

source 'https://rubygems.org'

ruby ENV['OSEM_RUBY_VERSION'] || '2.5.0'

# rails-assets requires >= 1.8.4
if Gem::Version.new(Bundler::VERSION) < Gem::Version.new('1.8.4')
  abort "Bundler version >= 1.8.4 is required"
end

# as web framework
gem 'rails', '~> 5.2.3'

# Use Puma as the app server
gem 'puma', '~> 3.0'

# respond_to methods have been extracted to the responders gem
# http://edgeguides.rubyonrails.org/upgrading_ruby_on_rails.html#responders
gem 'responders', '~> 2.4', '>= 2.4.1'

# as supported databases
gem 'mysql2'
gem 'pg'

# for tracking data changes
gem 'paper_trail'

# for upload management
gem 'carrierwave'
gem 'carrierwave-bombshelter'
gem 'mini_magick'

# for internationalizing
gem 'rails-i18n', '>= 5.1.3'

# as authentification framework
gem 'devise', '>= 4.7.1'
gem 'devise_ichain_authenticatable', '>= 0.3.2'

# for openID authentication
gem 'omniauth'
gem 'omniauth-facebook'
gem 'omniauth-github'
gem 'omniauth-google-oauth2'
gem 'omniauth-openid'

# Bot-filtering
gem 'recaptcha', require: 'recaptcha/rails'

# as authorization framework
gem 'cancancan'

# for roles
gem 'rolify'

# to show flash messages from ajax requests
gem 'unobtrusive_flash', '>= 3.3.1'

# as state machine
gem 'transitions', :require => %w( transitions active_record/transitions )

# for comments
gem 'acts_as_commentable_with_threading'
gem 'awesome_nested_set'

# as templating language
gem 'haml-rails', '>= 1.0.0'

# for stylesheets
gem 'sass-rails', '>= 5.0.7'

# as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'

# as the front-end framework
gem 'autoprefixer-rails'
gem 'bootstrap-sass', '~> 3.4.0'
gem 'cocoon'
gem 'formtastic', '~> 3.1.5'
gem 'formtastic-bootstrap', '>= 3.1.1'

# as the JavaScript library
gem 'jquery-rails', '>= 4.3.5'
gem 'jquery-ui-rails', '~> 4.2.1'

# for languages validation
gem 'iso-639'

# frontend javascripts
source 'https://rails-assets.org' do
  # for placeholder images
  gem 'rails-assets-holderjs'
  # for formating dates
  gem 'rails-assets-date.format'
  # for or parsing, validating, manipulating, and formatting dates
  gem 'rails-assets-momentjs'
  # for smooth scrolling
  gem 'rails-assets-jquery-smooth-scroll'
  # as color picker
  gem 'rails-assets-spectrum'
  # for color manipulation
  gem 'rails-assets-tinycolor'
  # for drawing triangle backgrounds
  gem 'rails-assets-trianglify'
  # for scroll way points
  gem 'rails-assets-waypoints'
  # for markdown editors
  gem 'rails-assets-bootstrap-markdown'
  # for select with icon
  gem 'rails-assets-bootstrap-select'
  gem 'rails-assets-markdown'
  gem 'rails-assets-to-markdown', '~> 3'
end

# as date picker
gem 'bootstrap3-datetimepicker-rails', '~> 4.17.47'

# data tables
gem 'ajax-datatables-rails', '>= 0.4.3'
gem 'jquery-datatables-rails', '>= 3.4.0'

# for charts
gem 'chartkick'

# for displaying maps
gem 'leaflet-rails', '>= 1.5.1'

# for user avatars
gem 'gravtastic'

# for country selects
gem 'country_select'

# as PDF generator
gem 'prawn-qrcode'
gem 'prawn-rails', '>= 1.2.0'

# for QR code generation
gem 'rqrcode'

# to render XLS spreadsheets
gem 'axlsx', git: 'https://github.com/randym/axlsx.git'
gem 'axlsx_rails', '>= 0.5.2'

# as error catcher
gem 'airbrake'

# to make links faster
gem 'turbolinks'

# for JSON serialization of our API
gem 'active_model_serializers', '>= 0.10.10'

# as icon font
gem 'font-awesome-rails', '>= 4.7.0.5'

# for markdown
gem 'redcarpet'

# as rdoc generator
gem 'rdoc-generator-fivefish'

# for visitor tracking
gem 'piwik_analytics', '~> 1.0.2'

# for recurring jobs
gem 'delayed_job_active_record'
gem 'whenever', :require => false

# to run scripts
gem 'daemons'

# to encapsulate money in objects
gem 'money-rails', '>= 1.13.3'

# for lists
gem 'acts_as_list'

# for switch checkboxes
gem 'bootstrap-switch-rails', '~> 3.0.0'

# for parsing OEmbed data
gem 'ruby-oembed'

# for uploading images to the cloud
gem 'cloudinary'

# for setting app configuration in the environment
gem 'dotenv-rails', '>= 2.7.5'

# configurable toggles for functionality
# https://github.com/mgsnova/feature
gem 'feature'

# For countable.js
gem "countable-rails", ">= 0.0.1"

# Both are not in a group as we use it also for rake data:demo
# for fake data
gem 'faker'
# for seeds
gem 'factory_bot_rails', '>= 4.11.1'

# for integrating Stripe payment gateway
gem 'stripe'

# Provides Sprockets implementation for Rails Asset Pipeline
gem 'sprockets-rails', '>= 3.2.1'

# for multiple speakers select on proposal/event forms
gem 'selectize-rails'

# For collecting performance data
gem 'skylight'

# Nokogiri < 1.8.1 is subject to:
# CVE-2017-0663, CVE-2017-7375, CVE-2017-7376, CVE-2017-9047, CVE-2017-9048,
# CVE-2017-9049, CVE-2017-9050
gem 'nokogiri', '>= 1.11.4'

# memcached binary connector
gem 'dalli'

# Use guard and spring for testing in development
group :development do
  # to launch specs when files are modified
  gem 'guard-rspec'
  gem 'haml_lint'
  gem 'spring-commands-rspec'
  # for static code analisys
  gem 'rubocop', require: false
  gem 'rubocop-rspec'
  # to open mails
  gem 'letter_opener'
  # as deployment system
  gem 'mina'
  # as debugger on error pages
  gem 'web-console', '>= 3.7.0'
  # as development database
  gem 'sqlite3'
end

group :test do
  # as test framework
  gem 'capybara', '>= 3.26.0'
  gem 'database_cleaner'
  gem 'geckodriver-helper'
  gem 'rspec-rails', '>= 3.6.1'
  gem 'transactional_capybara', '>= 0.2.0'
  gem 'webdrivers', '>= 4.1.3'
  # for measuring test coverage
  gem 'codecov', require: false
  # for describing models
  gem 'shoulda-matchers', require: false
  # for stubing/mocking models
  gem 'rspec-activemodel-mocks'
  # to freeze time
  gem 'timecop'
  # for mocking external requests
  gem 'webmock'
  # for mocking Stripe responses in tests
  gem 'stripe-ruby-mock'
  # For validating JSON schemas
  gem 'json-schema'
  # For using 'assigns' in tests
  gem 'rails-controller-testing', '>= 1.0.4'
  # For managing the environment
  gem 'climate_control'
  # For PDFs
  gem 'pdf-inspector', require: "pdf/inspector"
end

group :development, :test do
  # as debugger
  gem 'byebug'
end
