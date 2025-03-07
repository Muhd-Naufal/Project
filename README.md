# HELLO THERE!
This is a Read Me note inside every repository or a 'server'. This repository will assist in out CA2 project as it allows for real-time collaboration. And this is a just a note to inform anyone who comes by this page of what's this repository is about and contain.

## Files

- .gitignore
- PA2 R Markdown.Rmd
- PA2-Project.Rproj
- README.md
- Test File.R

As of 16/6/2019, there a a total of 5 files. I'll try to explain what each of these are.

> .gitignore

To be honest, I don't know what this file does but its name is a sequence of .git + ignore. This file was created while installing Git I believe and I guess you should ignore it since Git itself is telling you to ignore the file. 

> PA2 R Markdown.Rmd

This is a R Markdown file. This is different from a normal R file that we've been doing for the past couple of months. The formatting and output of the code is all different. Basically, think of this file as our 'report' that we will be submitting. So, most of the coding and work will be done in this file.

> PA2-Project.Rproj

This is the second file I can proudly say that I don't know what it does. *shrugs* 

> README.md

This file is the one you're reading now. Feel free to edit it and do whatever you want.

> Test File.R

Now this is a file you are familiar with. Its a normal R file but it's used to test out if the real-time collaboration of Git works after installation. You can ignore this or use this as a file to test whether your code works and whatnot.

## Git installation and GitHub synchronization
If there's ever an unfortunate incident that you simply lost your ability to Git or you had to hard reset your computer or whatever, this section will help in installing the whole thing again so we can all code together and be happily ever after!

### Links
- [Git](https://git-scm.com/downloads) - A Version Control System 
- [GitHub](https://github.com/) - Code hosting platform for collaboration 
- [GitHub Repository](https://github.com/Muhd-Naufal/PA2-Project) - Link to Repository

### Install Git
First, download Git and install it. Click next and leave everything on default until you've reached this page:

![1](https://user-images.githubusercontent.com/51323038/59566775-4eeb0f80-9097-11e9-8ba0-912aed2250d4.PNG)

Click on the top box because you only need Git Bash and nothing else. Afterwards, click next until you've reached this page:

![1](https://user-images.githubusercontent.com/51323038/59566818-b739f100-9097-11e9-995a-0fdb34ab32eb.PNG)

Just ignore it and proceed to install Git. After you're done. Git Bash should be installed on your computer. Now don't touch it, we'll get back to it later. 

### Create GitHub account
Head to GitHub and create an account. Make sure to choose the free account option and you can bullshit your personal preferences. Now, its important to remember your account name and password because you're going to need it on Git Bash and R Studio to push an update to the server. Don't worry you only need to do this once. 

### Git Bash
Alright once you've created a GitHub account, open up Git Bash and it should look something like this:

![3](https://user-images.githubusercontent.com/51323038/59566941-4eec0f00-9099-11e9-97d6-899a4d2858c2.PNG)

Ooo scary colour codey stuff. Nah don't fret because it's not gonna hack into your computer or anything. All it's going to do is to communicate to GitHub servers and authenticate your account from Github with Git something like that.

For communication to happen you need to input your GitHub particulars. That's where your account name and password comes in. After the $ sign, type in this line of code: 

> git config --global user.name "Your Name"

Inside the quotation marks you put in your account name from GitHub and then press enter. Nothing should happen and another line of code identital to the first one appears. Now type in this line of code but instead of your account name, type in your email address you linked with GitHub and press enter.

> git config --global user.email "Your Email"

Another same line of code should appear and you're done. You can close Git Bash now. Just in case, tt should look like this at the end:

![4](https://user-images.githubusercontent.com/51323038/59567065-22d18d80-909b-11e9-949b-35e8e6d89d7e.PNG)

### GitHub synchronization
Now for the important bit. Open up RStudio and click on File > New Project > Version Control

![5](https://user-images.githubusercontent.com/51323038/59567120-f5d1aa80-909b-11e9-9086-356d265968f5.PNG)

Click on Git and it should bring you to this window:

![6](https://user-images.githubusercontent.com/51323038/59567143-38938280-909c-11e9-8ed9-30c4d28449fb.PNG)

Leave it there first and head to the GitHub repository which looks something like this:

![7](https://user-images.githubusercontent.com/51323038/59567158-7b555a80-909c-11e9-8823-abb815879beb.PNG)

(If you don't have, I think you need permission from the owner of the repository. That person needs to share it by sending an invite link. It's under Settings > Collaborators)

You see on the right hand side of the screen where there is a green button called 'Clone or download'. Click on it and copy the URL and then paste it on RStudio with the open Git version control window. 

![8](https://user-images.githubusercontent.com/51323038/59567189-13ebda80-909d-11e9-8697-89b99159b4a1.PNG)

Click create project and after a bit of loading, Git/GitHub/RStudio should all now be synchronized. If everything goes well, your toolbar should now have a Git button. And if you noticed, your files are changed to match this repository. The same files on GitHub are now on your computer. This means whatever changes you do will now be reflected on the repository or server.

![9](https://user-images.githubusercontent.com/51323038/59567224-73e28100-909d-11e9-96de-01baf97245de.PNG)
![10](https://user-images.githubusercontent.com/51323038/59567281-30d4dd80-909e-11e9-9994-d841b9edc762.PNG)

# How it works
I'll keep this short because it's hard to demonstrate how the real-time collaboration works without a second person to view the changes.

Basically, you need to know this three things:
- Commit
- Pull
- Push

## Commit
Commit is just saving the action that you've done. If you added couple line of code and satisfied that it works, you commit those changes. You deleted some lines of redundant codes, you commit those changes. It's like a save button but this time you're saving those changes before Pushing those changes. 

There will always be a text box telling you to type the commit text. The text is usually short and simple. It's just a way to inform others what changes you made to the file. So when others update their own file to the latest version and saw something different, they can refer to the commit text to see what changes has been applied by the latest user and why that user made those changes. Try to make it a habbit to comment. 

## Pull
Pull, like the name implies, pull any updates from the repository. If someone has added additional codes to the R file and pushed it to the repository, you want to be able to see it on your computer too. So all you do is to press the Pull button and it'll pull any updates and it'll apply on your file. 

## Push
Push is the opposit of Pull. Instead of Pulling any updates from the repository, you are the one now making changes to the R file and want to share it with others. But before you Push, remember that you have to commit those changes to inform others what have you added on the R file. Then you can proceed to Push. If it's your first time Pushing, a window will appear to input your GitHub particulars. After you're done you can now Push. 

# Important things to take note of!
## Save before committing
Before you commit, remember to save your file. It's the normal save (Ctrl + S). You'll find that you cannot commit because Git/GitHub found nothing to commit even though you made changes to the R file. It's just normal save and commit is not the same thing. To know if you haven't save, the file name should appear red

![11](https://user-images.githubusercontent.com/51323038/59567725-e8b8b980-90a3-11e9-87eb-5b17c9df441d.PNG)

## Choose the file that you want to commit and make sure it's tick

In the commit window, on the top left hand side contains the box where it'll show what kind of files has been changed. For this case, since I made changes to Test File only, so only that file appears and I must click on it to tell Git/Github that this is the file I want  to commit/update/Push. If I made changes to multiple files, those multiple files will appear there and just click on the files you want to commit/update/Push.

![12](https://user-images.githubusercontent.com/51323038/59567788-dd19c280-90a4-11e9-9b88-669910f98c15.PNG)

## Dark Square box ≠ tick box
![13](https://user-images.githubusercontent.com/51323038/59567846-a7290e00-90a5-11e9-857f-a903fca3e5cc.PNG)

Don't be deceived. That dark box doesn't mean that the file is selected. You must make sure that the file has a tick before proceeding. Just click on the box again or twice then the tick should appear.

# 2025 Update

It has been a while. Realize that the markdown file doesn't work anymore as the rgeos package is depreceated. However it can still work, we just have to force it to install the package.

1. Download the [Rtools Development Tool](https://cloud.r-project.org/bin/windows/Rtools/rtools44/rtools.html)
2. Install it in PATH. I did it via command prompt
- Open Command Prompt as Administrator.
- Add the Rtools path with the following command:
> setx PATH "%PATH%;C:\Rtools43\usr\bin"
- Restart your Command Prompt or R session.
4. Install rgeos - Type it in Rstudio console
> install.packages("remotes")
> remotes::install_version("rgeos", version = "0.6-4")
5. Test installation
> library(rgeos)
rgeos::version_GEOS()

It should come out with version. Then you're good to go to run the markdown files. Happy roaming!

