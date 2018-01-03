# Fork Development

* make the fix on a fix branch and use it later for a pull-request
* switch to the `dev-fork` branch
* `git cherry-pick` the fix commit
* update gem version under `lib/fog/openstack/version.rb`
* build the new gem with `bundle exec rake build`
* use the gem in the openstack-cpi and test it
* open a pr with the new fix against `fog-openstack`