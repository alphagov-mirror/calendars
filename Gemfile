source "https://rubygems.org"

ruby File.read(".ruby-version").chomp

gem "rails", "~> 5.2.4"
gem "rails-i18n", "~> 5.1.3"

gem "json", "~> 2.3.0"
gem "plek", "3.0.0"

gem "govuk_publishing_components", "~> 21.43.0"

gem "rack_strip_client_ip", "0.0.2"

gem "sass-rails", "5.0.7"
gem "uglifier", "4.2.0"

if ENV["SLIMMER_DEV"]
  gem "slimmer", path: "../slimmer"
else
  gem "slimmer", "~> 13.3.0"
end

if ENV["API_DEV"]
  gem "gds-api-adapters", path: "../gds-api-adapters"
else
  gem "gds-api-adapters"
end

group :test, :development do
  gem "pry-byebug"
  gem "rubocop-govuk"
  gem "scss_lint-govuk"
end

group :test do
  gem "capybara", "3.32.1"
  gem "govuk-content-schema-test-helpers", "~> 1.6.1"
  gem "govuk_test"
  gem "mocha", "1.11.2", require: false
  gem "rails-controller-testing"
  gem "rspec-rails", "~> 4.0.0"
  gem "shoulda", "3.6.0"
  gem "simplecov", "0.18.5"
  gem "simplecov-rcov", "0.2.3"
  gem "timecop", "0.9.1"
  gem "webmock", "~> 3.8.3"
end

# Upgrade to Sentry
gem "govuk_app_config", "~> 2.1.2"
