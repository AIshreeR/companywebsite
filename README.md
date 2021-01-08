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
### Step 7:
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
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contact">Contact Us</a></div> 
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
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c3.jpg"  alt="product image">
            </div>
            <div class="itemname">Graphic card</div>
            <div class="itemprice">Price: Rs.20000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c4.jpg"  alt="product image">
            </div>
            <div class="itemname">RAM RGB</div>
            <div class="itemprice">Price: Rs.6000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c5.jpg"  alt="product image">
            </div>
            <div class="itemname">speaker</div>
            <div class="itemprice">Price: Rs.7000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c6.jpg"  alt="product image">
            </div>
            <div class="itemname">mouse</div>
            <div class="itemprice">Price: Rs.3000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c7.jpg"  alt="product image">
            </div>
            <div class="itemname">Intel i9 9900k Processor</div>
            <div class="itemprice">Price: Rs.54000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c8.jpg"  alt="product image">
            </div>
            <div class="itemname">128 GB pendrive</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c9.jpg"  alt="product image">
            </div>
            <div class="itemname">SATA SSD (samsung)</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c10.jpg"  alt="product image">
            </div>
            <div class="itemname">RGB color keyboard</div>
            <div class="itemprice">Price: Rs.25000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c11.jpg"  alt="product image">
            </div>
            <div class="itemname">Headset</div>
            <div class="itemprice">Price: Rs.15000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c12.jpg"  alt="product image">
            </div>
            <div class="itemname">IOT - board</div>
            <div class="itemprice">Price: Rs.7000.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### people.html:
```
{% extends "website/base.html" %}

{% block content %}
    <div class="people1">
    <h1>People Working In Silicon Private Limited:</h1>    
    </div>
    
    <div>
        <h3><u>President:</u></h3>
        <p>Natasha Maris</p>
        <img src="/static/img/natasha.jpg">
    </div>

    <div>
        <h3><u>Vice President:</u></h3>
        <p>Yun Shu</p>
        <img src="/static/img/yunshu1.jpg">
    </div>

    <div>
        <h3><u>Director:</u></h3>
        <p>Kathryn Doris</p>
        <img src="/static/img/kathryn.jpg">
    </div>

    <div class="people2">
        <h3><u>Members:</u></h3>
        <p>Declan Lynch</br>
        Front-End Development</p>
        <img src="/static/img/declan.jpg">
    </div>
    <div>
        <p>Cynthia Myers</br>
        Back-End Development</p>
        <img src="/static/img/cynthia.jpg">
    </div>
    <div>
        <p>Richmond Frazier</br>
        Technical Lead</p>
        <img src="/static/img/richmond.jpg">
    </div>
    <div>
        <p>Tang Xue</br>
        Technical Lead</p>
        <img src="/static/img/tangxue.jpg">
    </div>
    <div>
        <p>Hina Sakura</br>
        Design Team Lead</p>
        <img src="/static/img/hina.jpg">
    </div>
    <div>
        <p>Dong-hyun</br>
        Marketing Team Lead</p>
        <img src="/static/img/dong.jpg">
    </div>
{% endblock  %}
```
### contact.html:
```
{% extends "website/base.html" %}

{% block content %}
    <div class="people1">
        <h1>Contact Us:</h1>    
    </div>

    <div>
    <form action="//submit.form" id="ContactUs100" method="post" onsubmit="return ValidateForm(this);">
    <script type="text/javascript">
    function ValidateForm(frm) {
    if (frm.Name.value == "") { alert('Name is required.'); frm.Name.focus(); return false; }
    if (frm.FromEmailAddress.value == "") { alert('Email address is required.'); frm.FromEmailAddress.focus(); return false; }
    if (frm.FromEmailAddress.value.indexOf("@") < 1 || frm.FromEmailAddress.value.indexOf(".") < 1) { alert('Please enter a valid email address.'); frm.FromEmailAddress.focus(); return false; }
    if (frm.Comments.value == "") { alert('Please enter comments or questions.'); frm.Comments.focus(); return false; }
    return true; }
    </script>
    <table style="width:100%;max-width:550px;border:0;" cellpadding="8" cellspacing="0">
    <tr> <td>
    <label for="Name">Name*:</label>
    </td> <td>
    <input name="Name" type="text" maxlength="60" style="width:100%;max-width:250px;" />
    </td> </tr> <tr> <td>
    <label for="PhoneNumber">Phone number:</label>
    </td> <td>
    <input name="PhoneNumber" type="text" maxlength="43" style="width:100%;max-width:250px;" />
    </td> </tr> <tr> <td>
    <label for="FromEmailAddress">Email address*:</label>
    </td> <td>
    <input name="FromEmailAddress" type="text" maxlength="90" style="width:100%;max-width:250px;" />
    </td> </tr> <tr> <td>
    <label for="Comments">Comments*:</label>
    </td> <td>
    <textarea name="Comments" rows="7" cols="40" style="width:100%;max-width:350px;"></textarea>
    </td> </tr> <tr> <td>
    * - required fields
    </td> <td>
    <input name="skip_Submit" type="submit" value="Submit" />
    </td> </tr>
    </table>
    </form>
    </div>

    <div class="people3">
        <h4><u>Consultants:</u></h4>
        <p>Dougal Henderson</br>
        Phone Number: +91 7383378342</br>
        Email Id: dougalhenderson@gmail.com</p>

        <p>Gustave Ilyes</br>
        Phone Number: +91 7839362848</br>
        Email Id: gustave011@gmail.com</p>

        <p>Areum Bong-Cha</br>
        Phone Number: +91 8394848483</br>
        Email Id: areum890@gmail.com</p>
    </div>
{% endblock  %}
```

## OUTPUT:
![output](./static/img/output1.jpg)

![output](./static/img/output2.jpg)

![output](./static/img/output3.jpg)

![output](./static/img/output4.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/report1.jpg)

## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://demo2.student.saveetha.in:8000/. HTML code is validated.