
# Guide on how to Host a Resume on Github Pages

The purpose of this README is to help the user to host as well as format a resume using software stack such as Github Pages, Jekyll, Markdown, and Visual Studio Code

- [Requirements](#Requirements)
- [Instructions](#instructions)


## Requirements
Before proceeding with the instructions, there are a few requirements that has to be met.

- Github Account
  - A Github account allows the user to store codes in different repositories and you will be able to use Github pages as well.
  - [Sign up for free](https://www.github.com/)
 
- Ruby, Jekyll and GitBash
  - Download [Ruby](https://www.ruby-lang.org/en/downloads/)
  - Run command: "ruby -v" to check if ruby has been installed.
  - Download [Jekyll](https://jekyllrb.com/docs/installation/)
  - Run command: "jekyll -v" to check if jekyll has been installed.
  - Download [Gitbash](https://git-scm.com/downloads)
  
- Resume(Jekyll templates)
  - Jekyll Template: You can download a free template from [here](https://jekyllthemes.io/free). Andrew Etter(Page 51) describes Jekyll as a "robust system for generating nested navigation menus" as it is was developed specially for documentations. All the templates will redirect you to the github page where you can either clone it to your local repository or fork it to your github page. Using fork is easier as the you dont have to use command line but I will show how to do both ways.
  - For local computer
    - Once downloaded, Open command prompt and navigate the folder where you downloaded the template.
    - On Command prompt, once reached the folder, Run: Bundle install
    - Once downloaded, Run: buncle exec jekyll serve
    - After this, a link will pop up, copy that and paste it on any web browser to see the template.

- Markdown Editor
  - You will have to make your resume in Markdown format. If you choose to make a resume from scratch and not use a jekyll template, the following link will give you some head start on how to use Markdown
  

## Instructions(using Fork)
![Image](https://github.com/Vedant1206/Vedant1206.github.io/blob/gh-pages/images/Recording%202022-11-01%20at%2017.05.04.gif)

- First, the user has used the Fork command, clone it locally on github, and then they can easily change the template by opening the files directly on their github and commiting it once the changes has been made
- Most of the basic customization will take place in the `/_config.yml` file. Here is a list of customizations available via _config.yml
- For editing content, most of the content configuration will take place in the `/_layouts/resume.html` file. Simply edit the markup there accordingly
- For changing photo, click on images folder, and paste any image and rename it as avatar.jpg

## Instructions(using Local Computer)

### Step 1) Open Github and Create Repository
- Once signed into the github account, you will see an option "Repositories" and click on it.
- A new page will pop up where you will see a green button on the right hand side that says "New". Click on it.
- In the repository name, type "[your-github-name].github.io".
- Click on Create Repository
- Andrew Etter mentiones "GitHub Flavored Markdown is a popular and fine choice for simple webbased help systems."(Page 40)

### Step 2) Clone repository on your local computer
- On your github account, click on the github repository that you made earlier.
- You will see a green color button saying code. Click on that. 
- Copy the link and open the folder where you want to clone this repo.
- Once the folder is open, right click and click on "git bash here".
- type- git clone "link that you coppied" and press enter. The repo will be created.
- Andrew Etter mentiones "Developers are more likely to contribute if they don't have to clone a separate repository,"(Page 46). This is why we have make a clone of the github repository to avoid any other confusions. 


### Step 3) Bundle install
- Using command line, cd to the directory where you cloned the repository.
- Once reached, type "bundle install".
- Once downloaded, type "bundle exec jekyll serve".
- Open your browser to `localhost:4000`

### Step 4) Customize suitable resume
- Most of the basic customization will take place in the `/_config.yml` file. Here is a list of customizations available via _config.yml
- For editing content, most of the content configuration will take place in the `/_layouts/resume.html` file. Simply edit the markup there accordingly
- For changing photo, click on images and paste any image and rename it as avatar.jpg

### Step 5) Pushing the data on Github
- After making the changes, now you have to push the data back to github repo. 
- To do this, again run git bash and paste the folowing commands in sequence
  - git add .
    -(If there is an error, type git status, if you see red colored text, type git add "red colored text". This should be done for everyfile that wasn't added manually and one by one)
  - git commit -m "added files"
  - git push origin master

### Once Either of the instruction are completed, The resume has been successfully hosted and the user can open it by typing- github-username.github.io 

## More Resources(using Local Computer)
- For additional help regarding Markdown, here is a [Cheat Sheet](https://www.markdownguide.org/cheat-sheet/) and a [Markdown Tutorial](https://www.markdowntutorial.com/) for better understanding
- For additional help with using Git and Git bash, here is a [link](https://www.youtube.com/watch?v=USjZcfj8yxE)
- Andrew Etter’s Modern Technical Writing will be a good source to understand about [Techical writing(https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)

## Authors and Achnowledgements
- Authored by Vedant Pulahru
- Template forked from Joel Glovier [Github](https://github.com/jglovier)
- Thanks to my group members
  - [Taylor Roy](https://github.com/TayRoy)
  - [Josh Sigurdson](https://github.com/joshsig)
  - [Mansimar Bhasin](https://github.com/mansimars)

## FAQ
### Why is Markdown better than a word processor
- While word processor offers a lot of toolbars, they often gets inconvinient. Markdown is an easy language to learn and helps in getting rid of most of the inturuption for the user. According to Andrew Etter(Page 40) "Markdown is popular and fine choice for simple web based help systems" 
### Why is my resume not showing up
- If you are having difficulties running this resume website, there may be many reasons for that. Make sure of the following points
  - Make sure there is no syntax error
  - If used local computer, make sure everyting was pushed.
  - make sure the resume is in md format.
