# Welcome to the {{config.site_name}}!

This is the [ribbity](https://github.com/ctb/ribbity) sandbox site!

This site is automatically generated from the [ribbity-sandbox issue
tracker] on GitHub.

To give it a try -

first, [create a new issue](https://github.com/ribbity-org/ribbity-sandbox/issues/new?assignees=&labels=&template=add-a-new-page-.md&title=). Don't worry about the content, just throw in some markdown!

Then, count to 30 while GitHub Actions rebuilds the site.

Finally, reload this site and search for your new issue!

## Start here!

{% for issue in issues_list %}
{% if issue.is_frontpage %}

[{{config.issue_title_prefix}}{{issue.title}}]({{issue.output_filename}})

{% endif %}
{% endfor %}

---

## [All examples](examples.md)

---

## [All categories](labels.md)

