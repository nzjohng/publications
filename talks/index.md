# List of Talks

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.name contains '/talks/' %}
 - [{{ file.path }}]({{ site.url }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
        
