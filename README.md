# Technical Documentation

[![Build Status](https://travis-ci.com/alphagov/verify-tech-docs.svg?branch=master)](https://travis-ci.com/alphagov/verify-tech-docs)

This repository is the source for the [GOV.UK Verify technical documentation website][verify].

This project uses the [Tech Docs Template][template], which is a [Middleman template][mmt] that you can use to build technical documentation using a GOV.UK style.

👉 To find out more about setting up and managing content for a website using this template, see the [Tech Docs Template documentation][tdt-docs].

## Before you start

To use the Tech Docs Template you need:

- [Ruby][install-ruby]
- [Middleman][install-middleman]

## Making changes

To make changes to the documentation for the Tech Docs Template website, edit files in the `source` folder of this repository.

You can add content by editing the `.html.md.erb` files. These files support content in:

- Markdown
- HTML
- Ruby

👉 You can use Markdown and HTML to [generate different content types][example-content] and [Ruby partials to manage content][partials].

👉 Learn more about [producing more complex page structures][multipage] for your website.

## Preview your changes locally

To preview your new website locally, navigate to your project folder and run:

```sh
bundle exec middleman server
```

👉 See the generated website on `http://localhost:4567` in your browser. Any content changes you make to your website will be updated in real time.

To shut down the Middleman instance running on your machine, use `ctrl+C`.

If you make changes to the `config/tech-docs.yml` configuration file, you need to restart Middleman to see the changes.

## Publish your changes

Travis CI automatically publishes changes merged into the master branch of this repository.

## Troubleshooting

Run `bundle update` to make sure you're using the most recent Ruby gem versions.

Run `bundle exec middleman build --verbose` to get detailed error messages to help with finding the problem.

## Licence

Unless stated otherwise, the codebase is released under [the MIT License][mit].
This covers both the codebase and any sample code in the documentation.

The documentation is [© Crown copyright][copyright] and available under the terms of the [Open Government 3.0][ogl] licence.

[verify]: https://www.docs.verify.service.gov.uk
[mit]: LICENCE
[copyright]: http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/
[ogl]: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/
[mit]: LICENCE
[copyright]: http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/
[ogl]: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/
[template]: https://github.com/alphagov/tech-docs-template
[mmt]: https://middlemanapp.com/advanced/project_templates/
[tdt-docs]: https://tdt-documentation.london.cloudapps.digital
[multipage]: https://tdt-documentation.london.cloudapps.digital/multipage.html#build-a-multipage-site
[example-content]: https://tdt-documentation.london.cloudapps.digital/content.html#content-examples
[partials]: https://tdt-documentation.london.cloudapps.digital/single_page.html#add-partial-lines
[install-ruby]: https://tdt-documentation.london.cloudapps.digital/install_macs.html#install-ruby
[install-middleman]: https://tdt-documentation.london.cloudapps.digital/install_macs.html#install-middleman
