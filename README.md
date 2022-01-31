<meta name="google-site-verification" content="cGgjq3M1u6oI4PVYy-qFMCTnvU0hwT654XD8HE3zX4M" />


# Publications and documents
John Grundy's publications, talks, misc documents repository

List of collections:

{% assign doclist = site.pages | sort: 'url'  %}
    
       {% for doc in doclist %}
            {% if doc.name contains '.md' or doc.name contains '.html' %}
 - [{{ doc.url }}]({{ site.url }}{{ site.baseurl }}{{ doc.url }})
            {% endif %}
        {% endfor %}
    

    

