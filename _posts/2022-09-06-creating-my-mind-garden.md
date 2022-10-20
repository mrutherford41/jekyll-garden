---

layout: new
title: Creating My Mind Garden
categories: mind
published: false

---

### **Why?**
to avoid the time sink of social media

to create rather than react

to keep track of ideas and share knowledge 

<br>
<div style="border: 2px solid black; border-radius: 40px; width: 100%; "></div>
<br>
### **Where?**

<span style="font-weight: bold; color: white; background: black;">The Options I Didn't Use and Why</span>

CMS/Website Builder: **Wix**

The appeal of Wix was that it offered CMS features but upon learning more about other options I realized databases weren't something that was required and was more than I needed for this site.

Bare Bones: **HTML/CSS**

Basic HTML/CSS would be sufficent for the layout of a basic blog but the process of having to create new pages everytime I wanted to create a new post ruled this out. I also didn't want to mess with having to design from scratch.  

Static-site Generator: **Gastsby**

Static-site generators seemed to be the middle ground but Gatsby would require a little more time to learn about React components and GraphQL.

<br>
<span style="font-weight: bold; color: white; background: black;">What I Did Choose and Why</span>

The Winner: **Jekyll**

I had no experience with Jekyll before this and after installing I was able to make changes and easily create this site and get it up and running in a couple of days.

Only required me to learn a bit of Markdown and used some existing knowledge of html/css but not much.

<br>
<div style="border: 2px solid black; border-radius: 40px; width: 100%; "></div>
<br>
### **How?**

Note: These instructions are using Windows 10.

<span style="font-weight: bold; color: white; background: black;">Installing Ruby</span>

1. Download the ruby installer [here](https://rubyinstaller.org/downloads/)

2. Run installer and follow the steps shown in the command prompt window

3. 



<span style="font-weight: bold; color: white; background: black;">Installing Git</span>

[Install Git Tutorial](https://www.atlassian.com/git/tutorials/install-git#windows)

 
	$ git config --global user.name "Your Name" 

	$ git config --global user.email "youremail@email.com"

<span style="font-weight: bold; color: white; background: black;">Installing Jekyll</span>

open a new command prompt (run as administrator)

install jekyll bundler

	$ gem install jekyll bundler

check to make sure jekyll has been installed properly

	$ jekyll -v

cd to the location you want to create your new directory where all your files will be created

create a new jekyll site

	jekyll new "nameofdirectory"

Note: when I first ran this code I got an error and after some googling I came across this fix and it worked for me.
> 


<span style="font-weight: bold; color: white; background: black;">Editing Pages</span>



When creating a new site the 'minima' theme is already applied which worked for me. I didn't want to worry about the design as much as the structure of my site so I didn't mess with any styling. It is possible to create any style you would like or to use themes that have already been made by others and are availabe to use.

<span style="font-weight: bold; color: white; background: black;">Create a Git Repository</span>

1. Go to your Github Account and click '+' in the top right of the header

2. 'Create New Repository'

3. Give it a name and click 'save'

4. Get the url which will be used in the next few steps (ex. https://githubusername.respositoryname.git)

<span style="font-weight: bold; color: white; background: black;">Pushing to Github</span>

Make sure you are in the top folder for your site and run the following commands


	$ git init

	$ git checkout -b gh-pages

	$ git status

	$ git add .

	$ git commit -m "description"

	$ git push origin gh-pages


<span style="font-weight: bold; color: white; background: black;">Pushing Changes and New Pages</span>

Whenver you add new page or make any changes and are ready to show them on your published site you just need to run these commands and they will be live:

It should take just a few seconds for any changes to show up on your published site.

	$ git add .

	$ git commit -m "new commit"

	$ git push origin gh-pages

<br>
Your site is now published and ready to gain an audience. There are many more features that I didn't cover including creating your own style or using already made themes. If that's something you would like to do I recommend these sites to learn more:


<br>
<br>
<span style="font-weight: bold; color: white; background: black;">Resources</span>

- [Jekyll Tutorial Playlist by Mike Dean](#) This Youtube channel has the most straightforward and easiest tutorials to help you setup your first Jekyll site.
- [Markdown Basics](#)  

