###############################################
# Basic Rails3 template:
#
# *) install gems
# *) remove unnecessary files
# *) get rails.js for jquery
# *) change javascript :defaults 
# *) initial git commit
# *) create remote repo
# *) push code to remote repo
#
###############################################

# Gems
gem 'kaminari'
gem 'jquery-rails'

remove_file 'public/javascripts/controls.js'
remove_file 'public/javascripts/dragdrop.js'
remove_file 'public/javascripts/effects.js'
remove_file 'public/javascripts/prototype.js'
remove_file 'public/javascripts/rails.js'
remove_file 'public/index.html'
remove_file 'public/images/rails.png'

run 'wget http://github.com/rails/jquery-ujs/raw/master/src/rails.js -O public/javascripts/rails.js'
insert_into_file("config/application.rb",
                 "    config.action_view.javascript_expansions[:defaults] = %w(rails)\n",
                 :after => "# config.action_view.javascript_expansions[:defaults] = %w(rails)\n")

# jQuery & jQuery UI
generate 'jquery:install --ui'
insert_into_file('app/views/layouts/application.html.erb',
                 "<%= stylesheet_link_tag 'http://ajax.googleapis.com/ajax/libs/jqueryui/1.8.2/themes/start/ui.all.css' %>\n",
                 :before => "<%= stylesheet_link_tag :all %>")

# setup Capistrano
capify!

# Modify .gitignore
insert_into_file('.gitignore', 'Capfile\nconfig/deploy.rb\n', :after => 'tmp/\n')

# Initial git commit
git :init
git :add => "."
git :commit => "-a -m 'initial commit'"
git :clone => "--bare .git /tmp/#{app_name}.git"
# gitserver is only placeholder for your .ssh/config host
#run "scp -r /tmp/#{app_name}.git gitserver:/data/git/#{app_name}.git"
remove_file "/tmp/#{app_name}.git"
#git :remote => "add <gitserver name> <url to git repo>"
#git :push => "gitserver master"

say <<-eos
================================================================
TEMPLATE #{__FILE__} DONE.
================================================================
eos
