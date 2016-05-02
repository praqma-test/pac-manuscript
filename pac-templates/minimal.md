# {{title}}
{% for task in tasks.none %}
## {{task.task_id}} 
{% for commit in task.commits %}
 - {{commit.shortsha}}{% endfor %} 
{% endfor %}