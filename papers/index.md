# List of Papers

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.path contains 'papers' %}
 - [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
        
