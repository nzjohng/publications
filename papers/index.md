{% assign filelist2 = site.static_files | sort: 'path'  %}

         {% for file2 in filelist2 %}
            {% if file2.name contains '.pdf' and file2.path contains 'papers' %}
<link rel="canonical" href="{{ site.fullurl}}{{ file2.path }}" />
            {% endif %}
        {% endfor %} 

{% include google_analytics.html %}

# List of Papers

{% assign filelist = site.static_files | sort: 'path'  %}
    
       {% for file in filelist %}
            {% if file.name contains '.pdf' and file.path contains 'papers' %}
 - [{{ file.name }}]({{ site.fullurl }}{{ file.path }})
            {% endif %}
        {% endfor %}
        
        
