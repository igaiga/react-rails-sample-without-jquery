### rails new
- $ rails new react_rails_sample_without_jquery -J -T -B
  - -B skip bundle install
  - -T without testunit
  - -J without js lib

### Gemfile
```
gem 'react-rails', '~> 1.0'
gem 'haml-rails', '~> 0.9'
```

### config/application.rb
```
config.generators do |g|
  g.template_engine :haml # or :slim / :erb
  g.assets false
  g.helpers false
end
```

### react-rails
- $ rails g react:install
