Ronn-NG Developer's Guide
=========================

## Release checklist

* Update the version in files
  * ronn-ng.gemspec
  * `lib/ronn.rb`
* Update `CHANGES` with the release date
* Regenerate the man pages with `rake man`
* Run the tests one last time! `rake test`
* Commit the updated files
* Tag the release: `git tag vX.Y.Z`
* `git push --tags`
* Build and deploy the gem to RubyGems
  * ???
* TODO: Announce the release somewhere

After the release, start development on the next release:

* Update the version in files
  * ronn-ng.gemspec
  * `lib/ronn.rb`
* Update `CHANGES` with a new section for the next release
* Regenerate the man pages again: `rake man`
* Commit and push


## Running tests

`rake test` will run all the tests.

Do `RONN_QUIET_TEST=1 rake test` for shorter output that omits the possibly-long
diff outputs.