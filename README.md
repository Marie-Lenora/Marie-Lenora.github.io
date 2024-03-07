## How to Host a Resume Online using GitHub Pages ##

### Purpose ###
This document is written to to explain practical steps on how to format a resume using Markdown and host the formatted resume online using GitHub pages. The steps in this document would be related to the general principle of current technical writing as explained in Andrew Etter's book "[Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)"

In case you do not know what github or markdown is, I have included links to explain both items under more resources. I have also included the reason why this tutorial uses github pages to host the resume and not any other means. This follows the "Explain the what and why" principle of Andrew Etter's book.

### Prerequisites ###
* Understand Markdown basics. To learn how to use markdown, visit Markdown Tutorial under More Resources
* A resume formatted with markdown. See one [here].
* Own a github account. You can learn how to create one [here](https://learn.microsoft.com/en-us/visualstudio/version-control/git-create-github-account?view=vs-2022).
### Instructions ###
#### Hosting a Resume Online using Github Pages ####
1.  ##### Create a new Repository #####
    * In the menu bar under the username, click repositories
    * At the top right under the menu bar, click new
    * Name your repository username.github.io where username is the username of your github account
    * Add a description to help visitors understand more about your repository.
    * Set the repository to public
    * Scroll to the bottom and click create repository.
    
	![Steps to create a repository](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/896f71b8a761360dd3cf311b6ff22f210cfdf20d/Add%20resume%20to%20repository.gif)
 
     You have now successfully created a new repository that you will use to host your resume on github pages.

2. ##### Add resume to the created repository. #####
	As a prerequisite, you already have a resume that has been formatted with markdown. We will now be adding that resume to the repository we just created. 
	* On the codes tab of the Repository, under quick setup, click upload an existing file
	* In the window, either drag and drop your markdown resume file, or choose from file location as convenient.
	* Add a commit message. A commit message helps collaborators and visitors to understand changes to your repository. You can read more about commit messages [here](https://www.gitkraken.com/learn/git/tutorials/what-is-git-commit).
	* Click the commit changes button below.

3. ##### Set up GitHub pages #####
	* On the menu bar of your repository, go to settings
	* On the left school bar, Under the code and automation section, click pages
	* Your page should already be deployed. If it is not deplyed then follow the steps below: 
		* Under source, select deploy from branch
		* Choose the branch you want to deploy from, which for the purpose of this tutorial would be main.
		* Choose root directory
		* Click save
		
4. ##### Rename the Resume #####
	If you have finished setting up github pages ans you do not see your resume on the site, this is because github does not know which file to display. Github always displays the "index" file, so we will rename the resume to index.
	* On the code tab of the repository, select your resume by clicking the file name. 
	* At the top right of the preview dialog box, click the pencil button to go into edit mode.
	* Above the dialog box, edit the document name to index.md.
	* To the right of that, click commit changes
	* Enter your commint message
	* Click save.
	
	You should now have your resume completely hosted online now, you can preview it by visiting the website which would be username.github.io. It should look like this:
	
	
Now that we have successfully hosted the resume, we will add a jekyll theme to it.

#### Adding a Jekyll Theme to Hosted Resume ####
1. ##### Create the config file #####
	* In the codes tab of your github repository, click the "+" button on the menu bar
	* From the dropdown options, select create new file.
	* Name the file "_config.yml"
	* Add a line to the file "theme: Jekyll-theme-minimal"
	* Select commit changes.
	
	Your resume is now hosted with a jekyll theme. If you wish to use a different theme, you can view the lists of github supported jekyll themes [here](). Click on the theme of choice and you will be directed on how to add this theme to your github page. 
			
 
### More Resources ###
* Why Markdown: [How to Geek Article](https://www.howtogeek.com/why-you-should-be-writing-everything-in-markdown/)
* How to write the perfect Commit Message: [Git Tower article](https://www.git-tower.com/blog/how-to-write-the-perfect-commit-message/)
* What is Git? What is Github? [Coursera Article](https://www.coursera.org/articles/what-is-git)
* Why github pages: [dev.to article](https://dev.to/badbatunde/how-to-host-websites-on-github-pages-4113)

### Authors and Acknowledgements ###
Eseosa Ataga - Author

Aivee Toledo - Peer Reviewed this guide

Agape - Peer Reviewed this guide

Andrew Etter - Wrote the book, "Modern Technical Writing" whose principles were used in this guide.




### Frequently Asked Questions ###
1. ##### Q: Why is markdown better than using a word processor? #####

	A: One of the principles from Andrew Etter's book is to use a lightweight markup language. Markdown is the easiest markup language to learn for a beginner compared to HTML and XML. Asides that, documents produced using word processors e.g. .docx and .pdf files are very incompatible with website hosting. Further more, it is better to use distributed version control for long term technical documentation. This is because it saves it online and can easily be retrieved.
	
	
2. ##### Q: Why is my Resume not showing up? #####

	A: There are a couple of reasons why your resume might not show up. The first step would be to check that your repository is correctly named using the format: username.github.io. If that is correct, and you still cannot see your resume, check that the file in correctly named "index.md." Note that for github file names, the case is important as "Index.md" is different from "index.md."
	
	
