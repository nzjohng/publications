# List of Talks

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.path contains 'talks' %}
 - [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
        
