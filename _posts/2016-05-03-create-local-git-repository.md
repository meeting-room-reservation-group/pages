---
layout: post
title: Create Local Git Repository
---
Adding a (new) project to a new local git repository. 


## Action Plan

### Add Git Ignore File

There are many files, which should not be added to the git project repository, because they are configuration files for Eclipse, IntelliJ or output files from the Maven build, or other processes. Only those files that are can not be generated, should end up in a source repository.

Eclipse and IntelliJ can read Maven configuration files `pom.xml` to create their own specific configuration files.

Create the [git ignore](http://verhagen.github.io/git-tip-ignore-files/) file. 


### Add README

Every project should have a `README.md` which explains the general idea of the project, high level overview, links to important parts.

__TIP__ The file is written in [MarkDown](https://guides.github.com/features/mastering-markdown/) format. A simple text format with easy formatting rules.

Sample `README.md`

{% highlight markdown %}
# Project Title

This project ...
{% endhighlight %} 


### Create Local Git Repository

- Select in the window _Project Explorer_ or _Package Explorer_ the Eclipse project that should get in to git
- Use the context menu: _Team > Share Project..._  
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-00.jpeg)
- The dialog _Configure Git Repository_ will be shown  
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-01.jpeg)
- Select the check box _Use or create repository in parent folder of project_
- Select the row _meeting-roo..._ from the inner table _Project_ | _Location_ | _Repository_
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-02.jpeg)
- The check box _Project_ in that row can __not yet__ be selected
- Use the button _Create Repository_ at the bottom of the table
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-03.jpeg)
- This automatically set the check box for the _Project_ in the table
- Use the button Finish, to create the local git repository

__INFO__ Git only creates one directory `.git`, which is located in the root of the project. Inside that `.git` directory all configuration for git is stored as well as all the content (sources of the project).


### Add and Commit the Project Files to the Local Git Repository

- The Eclipse project as shown in the views _Package Explorer_ and _Project Explorer_ should now contain all the content with question mark `?` tags. This indicates that these files are not part of the git ignored files. And are ready to be added to the git repository, as sources of the project.  
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-04.jpeg)
- Use the context menu: _Team > Commit..._  
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-05.jpeg)
- The dialog _Commit Changes_ will be shown
- Fill in the _Commit message_ __Initial files__
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-06.jpeg)
- Verify that only _Files_ only those files are listed that should be added to the git repository
- Select all the check boxes, for the files that should be added, by this commit 
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-07.jpeg)
- Use the button _Commit_ to add the files to the local git repository
- When this is done, all files that are tracked by git, will have a small yellow cylinder, instead of a question mark
![Eclipse New Project Wizard]({{ site.url }}/images/eclipse/eclipse-create-local-git-repo-08.jpeg)
