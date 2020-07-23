###### rails apps deploying heroku
---




```
git clone git@github.com:takagotch/apptky4.1.3.git
rails new apptky4.1.3 -d postgresql  
cd apptky4.1.3
heroku create apptky4-1-3
// -d postgresql
// vi Gemfile
// gem 'sqlite3', group: [:deployment, :test]
// gem 'pg', group: :production    // gem 'pg', '>= 0.18', '< 2.0'
//
// vi config/environmens/production.rb
// rails_12factor
//  # Use a different logger for distributed setups.
//  # require 'syslog/logger'
//  # config.logger = ActiveSupport::TaggedLogging.new(Syslog::Logger.new 'app-name')
//  if ENV["RAILS_LOG_TO_STDOUT"].present?
//    logger           = ActiveSupport::Logger.new(STDOUT)
//    logger.formatter = config.log_formatter
//    config.logger    = ActiveSupport::TaggedLogging.new(logger)
//  end
//
// vi config/database.yml
// production:
//  url: <%= ENV['DATABASE_URL'] %>
rails g scaffold List name:string age:integer
rails db:create
rails db:migrate
rails s // rails s -b 192.168.33.10 -p 3000

git init
git add .
git commit -m "1st"
git remote
git remote add origin git@github.com:takagotch/apptky4.1.3git 
git push -u origin master
git push heroku master
heroku run rails db:migrate
```


```
git clone git@gitub.com:takagotch/apptky4.1.2.git
cd apptky4.git
heroku create apptky4.1.2
vi Gemfile
gem 'sqlite3', group: [:deployment, :test]
gem 'pg', group: :production

```


```
// git&heroku 
heroku create apptky4
git init
git add .
//
vi Gemfile
gem 'sqlite3', group: [:deployment, :test]
gem 'pg', group: :production
//
git comit -m "1st"
// New Repository - github
//: apptky4
// Create
// git remote
git remote add origin git@github.com:takagotch/apptky4.2.git // git remote
git push -u origin master
git push heroku master
heroku run rails db:migrate

```
https://apptky4.herokuapp.com/

---
###### 


```
rails g scaffold List name:string age:integer
rails g db:create
rails db:migrate
rails s -b 192.168.33.10 -p 3000
```

```
```



