source 'https://rubygems.org'
ruby '2.5.0'

# These gems take a long time to install.
# Thus, the "gem install" command is used in the Docker image creation
# process to preinstall these versions of these gems
# Version numbers are rigidly pinned to avoid a long wait after
# entering "bundle update".
gem 'ffi', '1.9.18'
gem 'nokogiri', '1.8.2'
gem 'pg', '0.21.0'
gem 'rails', '5.1.4'

gem 'autoprefixer-rails', '~> 7.2.5'
gem 'bcrypt', '~> 3.1.11'
gem 'bootstrap-sass', '~> 3.3.7'
gem 'devise', '~> 4.4.1'
gem 'geokit', '~> 1.11.0'
gem 'haml', '~> 5.0.4'
gem 'hashie', '~> 3.5.1'
gem 'jquery-rails', '~> 4.3.1'
gem 'puma', '~> 3.11.0'
gem 'rails_admin', '~> 1.2.0'
gem 'sass-rails', '~> 5.0.6'
gem 'validates_formatting_of', '~> 0.9.0'

group :development do
  gem 'guard-rspec', '~> 4.7.3'
  gem 'libnotify' if /linux/ =~ RUBY_PLATFORM
  gem 'growl' if /darwin/ =~ RUBY_PLATFORM
  gem 'spring', '~> 2.0.2'
  gem 'spring-commands-rspec', '~> 1.0.4'
end

group :development, :test do
  gem 'capistrano', '~> 3.10.0'
  gem 'capistrano-bundler', '~> 1.3.0'
  gem 'capistrano-rails', '~> 1.3.1'
  gem 'capistrano-rbenv', '~> 2.1.3'
  gem 'capistrano-rbenv-install', '~> 1.2.0'
  gem 'capistrano3-nginx', '~> 2.1.5'
  gem 'capistrano3-puma', '~> 3.1.1'
  gem 'dotenv-rails', '~> 2.2.0'
  gem 'faker', '~> 1.8.4'
  gem 'factory_bot_rails', '~> 4.8.2'
  gem 'pry-rails', '~> 0.3.4'
  gem 'rspec-rails', '~> 3.7.2'
end

group :production do
  gem 'rails_12factor', '~> 0.0.3'
end

group :test do
  gem 'capybara', '~> 2.17.0'
  gem 'capybara-slow_finder_errors', '0.1.4'
  gem 'codeclimate-test-reporter', '~> 1.0.4', require: nil
  gem 'database_cleaner', '~> 1.6.1'
  gem 'launchy', '~> 2.4.3'
  gem 'poltergeist', '~> 1.17.0'
  gem 'rails-controller-testing', '~> 1.0.2'
  gem 'selenium-webdriver', '~> 3.9.0'
end

# BEGIN: gems used in test_code.sh script
group :development, :testing do
  gem 'bundler-audit', '~> 0.6.0'  # Checks for vulnerable versions of gems
  gem 'brakeman', '~> 4.1.1' # Checks for security vulnerabilities
  gem 'sandi_meter', '~> 1.2.0' # Checks for compliance with Sandi Metz' four rules
  gem 'gemsurance', '~> 0.9.0' # Checks for outdated and insecure gems
end
# END: gems used in test_code.sh script

# BEGIN: for outline.sh
group :development do
  gem 'annotate', '~> 2.7.1' # Adds comments listing parameters and the output of "rails routes"
  gem 'railroady', '~> 1.5.2' # Generates block diagrams
  gem 'rails-erd', '~> 1.5.0' # Generates block diagrams
end
# END: for outline.sh
