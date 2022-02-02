# List of Talks

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.path contains 'talks' %}
 - [{{ file.name }}]({{ site.fullurl }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
        
