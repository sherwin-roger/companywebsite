# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Silicon Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/titleicon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Silicon Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a>People</a></div>
        <div class="menuitem"><a>Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Silicon Private Limited, Developed by Obed Otto.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/building2.jpeg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
## people.html:
```

{% extends "website/base.html" %}

{% block content %}

<div class="productcontent">    
    <h1>TOP BILLIONARES</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQM5vOtgPT6RTB08Tv8Rv_KwVVRJbEpFN8euA&usqp=CAU"  alt="product image">
            </div>
            <div class="itemname">BILL GATES</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="https://imgk.timesnownews.com/story/Mark-Zuckerberg_1.jpg?tr=w-1200,h-900"  alt="product image">
            </div>
            <div class="itemname">MARK ZUCKERBERG</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRlDarMXo5hYwk5_jMaTtsm7qh5nGdgT6_3Mw&usqp=CAU"  alt="product image">
            </div>
            <div class="itemname">ELON MUSK</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQHcI8pCYbvBFWzkN4rg18N2Z8be9z7Mth23g&usqp=CAU"  alt="product image">
            </div>
            <div class="itemname">JEFF BEZOS</div>
        </div>
    </div>
</div>
{% endblock  %}

```
## contact us.html

```
{% extends "website/base.html" %}

{% block content %}

<h1>FOR FURTHER DETAILS CONTACT US @</h1>
<div class="itemname">PHONE: 978820478</div>
<div class="itemname">EMAIL: silicon@gmail.com</div>

{% endblock  %}
```

## OUTPUT:
![output](./static/img/output1.jpg)

![output](./static/img/output1.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/report1.jpg)

![output](./static/img/report2.jpg)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://sherwin.student.saveetha.in:8000/. HTML code is validated.