source "https://rubygems.org"

chef_version = ENV.fetch("CHEF_VERSION", "11.10")

gem "chef", "~> #{chef_version}"
gem "chefspec", "~> 3.4" if chef_version =~ /^11/

gem "berkshelf", "~> 3.1.0"
gem "foodcritic", "~> 3.0.0"
gem "rake"
gem "rubocop", "~> 0.20.1"
gem "serverspec", "~> 1.3.0"

group :integration do
  gem "busser-serverspec", "~> 0.2.6"
  gem "kitchen-digitalocean", "~> 0.6.0"
  gem "kitchen-ec2", "~> 0.8.0"
  gem "kitchen-vagrant", "~> 0.14.0"
  gem "test-kitchen", "~> 1.2.1"
end
