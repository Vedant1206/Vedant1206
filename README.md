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
  - Jekyll Template: You can download a free template from [here](https://jekyllthemes.io/free). All the templates will redirect you to the github page where you can either clone it to your local repository or fork it to your github page. Using fork is easier as the you dont have to use command line but I will show how to do both ways.
  - For local computer
    - Once downloaded, Open command prompt and navigate the folder where you downloaded the template.
    - On Command prompt, once reached the folder, Run: Bundle install
    - Once downloaded, Run: buncle exec jekyll serve
    - After this, a link will pop up, copy that and paste it on any web browser to see the template.

- Markdown Editor using Sublime
  - As a coder, a text editor is very important. I, personally like to use [Sublime(download from here)](https://www.sublimetext.com/) because it is one of the best text editors as it allows us to code in any language possible and is user friendly.
  - You will have to make your resume in Markdown format. If you choose to make a resume from scratch and not use a jekyll template, the following link will give you some head start on how to use Markdown
  - [Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)

## Instructions(using Fork)

[Image](/images/Recording 2022-11-01 at 17.05.04.gif)
- Once the user has used the Fork command, They can easily change the template by opening the files directly on their github and commiting it once the changes has been made
- Most of the basic customization will take place in the `/_config.yml` file. Here is a list of customizations available via _config.yml
- For editing content, most of the content configuration will take place in the `/_layouts/resume.html` file. Simply edit the markup there accordingly
- For changing photo, click on images folder, and paste any image and rename it as avatar.jpg

## Instructions(using Local Computer)

### Step 1) Open Github and Create Repository
- Once signed into the github account, you will see an option "Repositories" and click on it.
- A new page will pop up where you will see a green button on the right hand side that says "New". Click on it.
- In the repository name, type "[your-github-name].github.io".
- Click on Create Repository

### Step 2) Clone repository on your local computer
- On your github account, click on the github repository that you made earlier.
- You will see a green color button saying code. Click on that. 
- Copy the link and open the folder where you want to clone this repo.
- Once the folder is open, right click and click on "git bash here".
- type- git clone "link that you coppied" and press enter. The repo will be created.

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
