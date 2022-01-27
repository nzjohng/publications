# List of Misc documents

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.path contains 'misc' %}
 - [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
