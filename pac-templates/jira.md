# PAC Changelog
{% for task in tasks.jira %}
## {{task.task_id}} 

### Summary

{{task.attributes.data.fields.summary}}
{% for commit in task.commits %}
 - {{commit.shortsha}}{% endfor %} 
{% endfor %}

