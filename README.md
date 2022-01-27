<meta name="google-site-verification" content="cGgjq3M1u6oI4PVYy-qFMCTnvU0hwT654XD8HE3zX4M" />

   {% assign doclist = site.pages | sort: 'url'  %}
    <ul>
       {% for doc in doclist %}
            {% if doc.name contains '.md' or doc.name contains '.html' or doc.name contains '.pdf' %}
                <li><a href="{{ site.baseurl }}{{ doc.url }}">{{ doc.url }}</a></li>
            {% endif %}
        {% endfor %}
    </ul>

# publications
John Grundy's publications repository
