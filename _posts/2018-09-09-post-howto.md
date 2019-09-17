---
layout: post
title: How to make posts for this site
permalink: /blog/2018-09-09-post-howto
---

## How to make a post for this site

- Write your post in markdown format. Here are [links](https://guides.github.com/features/mastering-markdown/) to [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) [guides](https://www.markdowntutorial.com/) for help with formatting
- Start with "front matter" This is what tells github that your document becomes a post and what title it is, where the link should go, and what tags you are going to use. You always need to say the layout is a post, and that the permalink is /blog/ and followed by the name of the post md file:  
` ---  `   
`layout: post`  
`title: Title of Post`  
`permalink: /blog/2019-09-09-post-name`  
`tags:`   
`- tag1`  
`- tag2`  
`--- `
- All of the md files have to be named with the correct convention: YYYY-MM-DD-Name-of-file.md
- Write the md file using the above links with any information you want to provide
- To use an image, copy this code and just change the name of the image. _NOTE: image names CANNOT have spaces in them_  
`![image]({{ site.baseurl}}/images/my-image-name.png)`
- If you are using a new primer/tag, tell Maggie and she will make a new page for the tag link

**Adding things to the site**

- First create a branch other then the master branch  
![one]({{ site.baseurl}}/images/first.png)
- Then in that branch go to the posts folder and click to add a new file  
![two]({{ site.baseurl}}/images/second.png)
- Then title your file with the naming convention and .md and copy and paste in your markdown file. Or you could just write it in here  
![three]({{ site.baseurl}}/images/third.png)
- Then click commit changes at the bottom of the page  
![four]({{ site.baseurl}}/images/fourth.png)
- Add an image by going to the image folder, adding a file via upload and commiting that addition  
![8]({{ site.baseurl}}/images/eigth.png)
- Then go to the code page for the branch you created, and click new pull request  
![5]({{ site.baseurl}}/images/fifth.png)
- **Make sure when you are doing a pull request it goes to my git up repository and not the person who created the website**  
![6]({{ site.baseurl}}/images/sixth.png)
- Then write a small message about what you are adding and click create pull request, the rest I should be able to do!  
![7]({{ site.baseurl}}/images/seventh.png)
