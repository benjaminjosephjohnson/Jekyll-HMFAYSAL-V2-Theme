---
layout: post
title:  "Using Python in AWS lambda"
date:   2018-06-23 14:59:56 -0700
categories: AWS
---
Let's make a lambda function! It's easier than you'd think. 

Navigate to the lambda service page to start the process.
![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 3.43.22 PM.png" | relative_url }})

Click on the 'create function' button in the top right.

![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 3.51.39 PM.png
" | relative_url }})

Author from scratch should be selected by default, if not, click on it at the top to select it.

Click the first dropdown to browse the selection of supported runtime environments and choose one that you are comfortable with. In this case I will choose python 3.6. 

![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 3.59.31 PM.png" | relative_url }})

Next we need to set the function's permissions, which we do by clicking on the Role dropdown panel. Click on 'create new role from template', and new fields will appear below.

Give the role a name, and choose 'Basic Edge Lambda permissions' from the policy templates. If you ever need to add permissions, you can go to IAM and edit the role later. 

![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 4.13.03 PM.png" | relative_url }})

The function is now ready to be created! Make sure you've given it a name before clicking on the create function button in the bottom left. 

You should see this page if you've done everything right.

![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 4.20.15 PM.png" | relative_url }})

Scroll down to the code page. This is the basic structure of a lambda function. You must have a function named lambda_handler, the output of your lambda function is what you return with your lambda_handler. Event can contain information about the thing that causes your lambda to run, and context can contain information about how your function performed when it ran. 

![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 4.27.39 PM.png" | relative_url }})

Let's try running it. 
Scroll up to the test button on the top of the page and click the dropdown near it to create a new test event.

![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 4.27.39 PM.png" | relative_url }})

Success! 

![My helpful screenshot]({{ "/assets/screenshots/Screen Shot 2018-06-23 at 8.41.10 PM.png" | relative_url }})

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
