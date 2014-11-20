# Ruby on Rails Tutorial: sample application

This is the sample application for
[*Ruby on Rails Tutorial: Learn Web Development with Rails*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/). You can use this reference implementation to help track down errors if you end up having trouble with code in the tutorial. In particular, as a first debugging check I suggest getting the test suite to pass on your local machine:

    cd /tmp
    git clone https://github.com/railstutorial/sample_app_rails_4.git
    cd sample_app_rails_4
    cp config/database.yml.example config/database.yml
    bundle install --without production
    bundle exec rake db:migrate
    bundle exec rake db:test:prepare
    bundle exec rspec spec/

If the tests don't pass, it means there may be something wrong with your system. If they do pass, then you can debug your code by comparing it with the reference implementation.

## Get Started in seconds

[![Hack railstutorial/sample_app_rails_4 on
Nitrous.IO](https://raw.githubusercontent.com/nanzhong/sample_app_rails_4/master/app/assets/images/no_hack_button_2_360.png)](#)

[![Deploy to Heroku](https://raw.githubusercontent.com/nanzhong/sample_app_rails_4/master/app/assets/images/no_heroku_button_2_360.png)](#)

[![Deploy to DigitalOcean](https://raw.githubusercontent.com/nanzhong/sample_app_rails_4/master/app/assets/images/deploy_to_do_button.png)](http://localhost:3001/droplets/new/?repo=nanzhong%2fsample_app_rails_4)
