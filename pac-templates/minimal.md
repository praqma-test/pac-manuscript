# PAC Changelog
{% for task in tasks.none %}
## {{task.task_id}} 
{% for commit in task.commits %}
 - {{commit.shortsha}}{% endfor %} 
{% endfor %}
{% if tasks.todo.size > 0 %}
## Todo list
{% for todo in tasks.todo %}
## {{todo.task_id}} 
{% for commit in todo.commits %}
 - {{commit.shortsha}}{% endfor %} 
{% endfor %}
{% endif %}
