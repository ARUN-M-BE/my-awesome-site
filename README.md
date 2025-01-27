  gem install bundler jekyll

  jekyll new my-awesome-site

  cd my-awesome-site

  bundle exec jekyll serve

# => Now browse to http://localhost:4000

Add Missing Gems to the Gemfile: Since the csv and logger libraries are no longer part of the default gems, you need to explicitly include them in your Gemfile. Open your project's Gemfile and add:

gem 'csv'
gem 'logger'

Install the Gems: After updating the Gemfile, run the following command to install the required gems:

bundle install
Update the Gemfile.lock: Running bundle install will automatically update your Gemfile.lock file to include the newly added gems.

Update the Gemfile.lock: Running bundle install will automatically update your Gemfile.lock file to include the newly added gems.

Verify the Jekyll Installation: Run the Jekyll command again to verify that the issue is resolved:

jekyll serve
Check Ruby Version Compatibility: Ensure you are using a compatible Ruby version for Jekyll (e.g., Ruby 2.7.x or 3.x). If you're using Ruby 3.4.0, ensure all gems in your project are compatible with this version.

Upgrade Jekyll (Optional): If the issue persists, consider upgrading Jekyll to the latest version, as it may have resolved this dependency issue in newer releases. You can update Jekyll by running:

gem update jekyll

If you're running Jekyll globally (not within a specific project), make sure to add csv and logger to your global gem environment by running:

gem install csv
gem install logger
If you're using a Ruby version manager like RVM or rbenv, ensure the correct Ruby version is active before making changes

