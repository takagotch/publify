### publify
---
https://github.com/publify/publify

```
bundle install
rake db:setup
rake db:migrate
rake db:seed
rake assets:precompile
rails server

heroku config:set PROVIDER=AWS
heroku config.set AWS_ACCESS_KEY_ID=<your_aws_access_key_id>
heroku config.set AWS_SECRET_ACCESS_KEY=<your_aws_secret_access_key>
heroku config.set AWS_BUCKET=<your_aws_bucket_name>

source 'https://rubygems.org'
ruby '2.4.3'
gem 'pg'
gem 'rails_12factor'
gem 'rails', '~> 5.2.0'

bundle install
git commit -am "Update bundle for Heroku"
web: bundle exec puma -c config/puma.rb

git add Procfile
git ci -m 'Tell Heroku how to run Rails'

heroku config:set SECRET_KEY_BASE=<your_generated_secret>
heroku run rake db:migrate db:seed
heroku restart

```

```

```

```
```


