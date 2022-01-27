# List of Papers

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.dir contains '/papers/' %}
 - [{{ file.path }}]({{ site.url }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
        
