{# receives 'issues_list', 'labels_to_issues', and 'piggy' #}

# Welcome to the Workshop Webpage for the Data Intensive Biology Lab

## [All workshops](examples.md)

{% for issue in issues_list %}
{% if issue.is_frontpage %}

[{{config.issue_title_prefix}}{{issue.title}}]({{issue.output_filename}})

{% endif %}
{% endfor %}

## [All categories](labels.md)
