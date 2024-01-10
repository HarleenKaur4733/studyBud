# Django
## Template Inheritance: 
Just rendering template is not the best thing. For example, I want to include navbar in every template, one option is to include navbar on every page. Another best option
is to use Template Inheritance. 

main.html
```
<body>
    {% include 'navbar.html' %}
    {% block content %}
    {% endblock content%}
  </body>
```

home.html
```
  {% extends 'main.html' %}
  {% block content %}
  <h1>Home Template</h1>
  {% endblock content %}
```
