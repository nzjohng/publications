# List of Theses

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.path contains 'theses' %}
 - [{{ file.name }}]({{ site.fullurl }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
