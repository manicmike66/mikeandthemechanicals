<style>
/* Dropdown Content (Hidden by Default) */
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #fff;
  color:#00C;
  min-width: 140px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
  width:100%;
  line-height:2rem;
  top:28px;
  list-style: none;
  text-align:center;
}

/* Links inside the dropdown */
.dropdown-content a {
  color: #00C;
  padding: 2px 6px;
  text-decoration: none;
  display: block;
}

/* Change color of dropdown links on hover */
.dropdown-content a:hover {background-color: #0d6efd;
    color: #fff;
}
#Toolbar ul { 
    list-style: none; 
    float: left; 
    padding:0;
}
#Toolbar ul li{ 
    font-size:small;
    border: 1px solid #003333;
}
/* Show the dropdown menu on hover */
.dropdown:hover .dropdown-content {
    display: block;
    }

/* Change the background color of the dropdown button when the dropdown content is shown */
.dropdown:hover .dropbtn {background-color: #001e36;}
</style>
<nav id="topnav"  class="navbar navbar-expand-sm navbar-dark my-4 border-top border-bottom border-white bootsnav" role="navigation">
    <ul class="nav navbar-nav mx-auto" data-in="fadeInDown" data-out="fadeOutUp"><!-- nav navbar-nav">-->
        {% assign navstyle = 'border border-white mx-2 bg-primary %}
        {% assign links = site.data.navigation %}
        {% for entry in links %}
            {% assign class = nav-item %}
            {% if page.url == entry.url %}
                {% assign class = 'nav-item active' %}
            {% endif %}
            {% if entry.sublinks %}
                <li id="{{entry.title}}_dropdown-menu" id="{{ class }}" class="{{ navstyle }} dropdown {{ class }} ">
                    <a href="{{ site.baseurl }}{{ entry.url }}" id="{{entry.title}}-link" class="text-emphasis nav-link h5 dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">{{ entry.title }} <span class="caret"></span></a>
                    <div class="dropdown-content" aria-labelledby="{{entry.title}}-link">
                        {% for sublink in entry.sublinks %}
                            <a class="dropdown-item" href="{{ site.baseurl }}{{ sublink.url }}">{{ sublink.title }}</a>
                        {% endfor %}
                    </div>
                </li>
            {% else %}
                <li id="{{ entry.title }}" class="{{ class }} {{navstyle}}">
                    <a class="nav-link h5 text-primary-emphasis" href="{{ site.baseurl }}{{ entry.url }}">{{ entry.title }}</a>
                </li>
            {% endif %}
        {% endfor %}
    </ul>
</nav>
