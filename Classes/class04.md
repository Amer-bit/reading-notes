# Links
links are created using 'a' element and 'href' attribute which stands 
for hyperlinks reference the browser show this element in rlined blue 
text by defualt. When linking to other website we include the full url 
of that website which is known as **Absolute URL** 

URL stand for *Uniform Resource locator* absolute URL starts with the 
domain name for that site, and can be followed by the path to a specific 
page. If no page is specified, the site will display the homepage.

When linking to other pages within the same site, you do not 
need to specify the domain name in the URL. You can use a shorthand 
known as a **relative URL**. These are like a shorthand version of 
absolute URLs because you do not need to specify the domain name 
Relative URLs help when building a site on your computer because you can 
create links between pages without having to set up your domain name or 
hosting.

## On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories

**NOTE: Refer to the Image on page 82** in this page u will see the directory strucutre The top-level folder is known as the root folder. (In this example, the root folder is called examplearts.) The root folder
contains all of the other files and folders for a website. Each section of the site is placed in a separate folder; this helps organize the files.

**Benifits of using relaive URL in your project**
- quicker to write
- because you can create links between pages when they are only on your personal computer (before you have got a domain name and uploaded them to the web)
- Because you do not need to repeat the domain name in each link

#### Email links 
using mailto To create a link that starts up the user's email program and
addresses an email to a specified email address, you use the <\a> 
element. However, this time the value of the href attribute starts
with mailto: and is followed by the email address you want the
email to be sent to. Like <\a href="mailto: user@ex.com">Your mail<//a>

#### Opening Links in a new window
we use target in href attribute to open links in new window 
we can link to a new window a specific part of the same page by using selectors (use id) in href attribute and link to specific part of the  page whether its on your site or on other one as long as the page has an ID attribute that identify specific part of the page