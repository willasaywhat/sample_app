# Ruby on Rails Tutorial: sample application

This is the sample application for
[*Ruby on Rails Tutorial: Learn Rails by Example*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).


Issues with the tutorial on (9/18/2010):

*	Beta 20 is the latest "stable" release of rspec-rails. Beta 22 has a bug wherein controller specs are not generated.

*	Webrat is not configured or installed by default in the tutorial. You have to add the gem to your Gemfile otherwise have_selector doesn't work.

*	On my particular machine, I had to install the Xcode tools in order for gems to build. Stupid mistake, but one that annoyed me for quite awhile.

*	The commands installed by gems, like rspec, don't work because they aren't automatically added to the path by bundler. Instead, you can do 'bundle exec rspec spec' and that works. rake spec will also achieve this, but you'd have to rake db:migrate before hand.