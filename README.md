Creating a New Noodall Component
================================
Instructions for extracting/creating a Noodall component gem

Setup
-----
Generate a new component/plugin template

  * `rails plugin new noodall-component-<name> --full -Om https://raw.github.com/stengland/noodall-plugin-template/master/template.rb`

This generates a Rails Engine and applies our customisations.

Process
-------
* Copy/create models in `app/models`

* Copy/create views in `app/views/admin/components` and `app/views/components`

* Setup slots for the new component under `test/dummy/config/initializers/noodall.rb`

* Add new slots to `test/dummy/app/models/content_page.rb`

* Add the new component slot to `test/dummy/app/views/nodes/content_page.html.erb`

* Add cucumber tests and/or unit tests

* Setup factories in `/factories`

* Fill in the `*.gemspec` file