<meta name="google-site-verification" content="cGgjq3M1u6oI4PVYy-qFMCTnvU0hwT654XD8HE3zX4M" />


# publications
John Grundy's publications repository


{% assign doclist = site.pages | sort: 'url'  %}
    
       {% for doc in doclist %}
            {% if doc.name contains '.md' or doc.name contains '.html' %}
 - [{{ doc.url }}]({{ site.baseurl }}{{ doc.url }})
            {% endif %}
        {% endfor %}
    

    

