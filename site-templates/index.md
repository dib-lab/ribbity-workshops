---
hide:
  - navigation
  - toc
---

{# receives 'issues_list', 'labels_to_issues', and 'piggy' #}

# Welcome to the Workshop Webpage for the Data Intensive Biology Lab

## [All workshops](examples.md)

{% for issue in issues_list %}

{{config.issue_title_prefix}} [{{issue.title}}]({{issue.output_filename}})

{% endfor %}

## [All topics](labels.md)

{% for label in labels_to_issues %}

{{label.description}} - [{{labels_to_issues[label]|length}} workshop]({{label.output_filename}})

{% endfor %}