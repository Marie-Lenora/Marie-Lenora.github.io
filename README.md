## How to Host a Resume Online using GitHub Pages 

### Purpose 
This document explains practical steps on how to format a resume using Markdown and host the formatted resume online using GitHub pages. The steps in this document would be related to the general principle of current technical writing as explained in Andrew Etter's book "[Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)"

In case you do not know what GitHub or markdown is, I have included links to explain both items under more resources. I have also included the reason why this tutorial uses GitHub pages to host the resume and not any other means. This follows Andrew Etter's book "Explain the what and why" principle.

### Prerequisites 
* Understand Markdown basics. To learn how to use Markdown, visit Markdown Tutorial under More Resources
* A resume formatted with markdown. See one [here](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/404efb4bf92a3095cfa4d3ce93a4668ef98dd7d8/index.md).
* Own a GitHub account. You can learn how to create one [here](https://learn.microsoft.com/en-us/visualstudio/version-control/git-create-github-account?view=vs-2022).
### Instructions
 #### Create a new Repository 
   1. In the menu bar under the username, click repositories
   2. At the top right under the menu bar, click the new button
   3. Name your repository username.github.io where the username is the username of your GitHub account
   4. Add a description to help visitors understand more about your repository.
   5. Set the repository to public
   6. Scroll to the bottom and click Create Repository.
    
![Steps to create a repository](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/896f71b8a761360dd3cf311b6ff22f210cfdf20d/Add%20resume%20to%20repository.gif)
 
 You have now successfully created a new repository that you will use to host your resume on GitHub pages.

#### Add a resume to the created repository. 
As a prerequisite, you already have a resume that has been formatted with markdown. We will now be adding that resume to the repository we just created. 
1. On the codes tab of the Repository, under quick setup, click Upload an existing file
2. In the window, either drag and drop your markdown resume file or choose from the file location as convenient.
3.  Add a commit message. A commit message helps collaborators and visitors understand changes to your repository. You can read more about commit messages [here](https://www.gitkraken.com/learn/git/tutorials/what-is-git-commit).
4. Click the `commit changes` button below.
	
	![How to add a resume to repository](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/e08e31aaf864a25a55c9aee3722de31b99d7fefa/Add%20resume%20to%20repository.gif)

#### Set up GitHub pages 
1. On the menu bar of your repository, go to settings
2. On the left school bar, Under the code and automation section, click pages
3. Your page should already be deployed. If it is not deployed then follow the steps below: 
	a. Under source, select deploy from branch
	
	b. Choose the branch you want to deploy from, which for this tutorial would be main.
			
	c. Choose the root directory
	
	d.  Click `commit changes`
		
	![How to set up github pages](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/e08e31aaf864a25a55c9aee3722de31b99d7fefa/Laumching%20Github%20pages.gif)
		
#### Rename the Resume 
If you have finished setting up GitHub pages and you do not see your resume on the site, this is because GitHub does not know which file to display. Github always displays the "index" file, so we will rename the resume to index.
1. On the code tab of the repository, select your resume by clicking the file name. 
2. At the top right of the preview dialogue box, click the pencil button to go into edit mode.
3. Above the dialogue box, edit the document name to index.md.
4. To the right of that, click Commit changes
5. Enter your commit message
6. Click `commit changes`.
	
![Rename the resume file](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/e08e31aaf864a25a55c9aee3722de31b99d7fefa/Change%20name%20of%20resume.gif)
	
You should now have your resume completely hosted online, you can preview it by visiting the website which would be username.github.io. It should look like this:

![Online hosted resume](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/e08e31aaf864a25a55c9aee3722de31b99d7fefa/Online%20hosted%20resume.gif)
	
	
Now that we have successfully hosted the resume, we will add a Jekyll theme to it.

#### Add a Jekyll Theme to Hosted Resume 

1. In the codes tab of your GitHub repository, click the "+" button on the menu bar
2.  From the dropdown options, select create new file.
3. Name the file `_config.yml`
4. Add a line to the file `theme: Jekyll-theme-minimal`
4. Select commit changes.
	
	![Adding a config file](https://github.com/Marie-Lenora/Marie-Lenora.github.io/blob/d27a3ae5683e76fc0439c6dab358bf81eea6d041/Create%20config%20file.gif)
	
	Your resume is now hosted with a Jekyll theme. You might not see the Jekyll theme immediately but that is fine as GitHub sometimes delays in updating the website. Give it a couple of minutes and refresh, you should see your theme reflected afterwards.
	
	 If you wish to use a different theme, you can view the lists of github supported jekyll themes [here](https://pages.github.com/themes/). Click on the theme of choice and you will be directed to a GitHub repository containing this theme. The Readme of this repository would give you instructions on how to apply that theme and all additional information needed.
			
 
### More Resources 
* Why Markdown: [How to Geek Article](https://www.howtogeek.com/why-you-should-be-writing-everything-in-markdown/)
* How to write the perfect Commit Message: [Git Tower article](https://www.git-tower.com/blog/how-to-write-the-perfect-commit-message/)
* What is Git? What is GitHub? [Coursera Article](https://www.coursera.org/articles/what-is-git)
* Why GitHub pages: [dev.to article](https://dev.to/badbatunde/how-to-host-websites-on-github-pages-4113)

### Authors and Acknowledgements 
Eseosa Ataga - Author

Aivee Teodocio - Peer Reviewed this guide

Agape Seo- Peer Reviewed this guide

Andrew Etter - Wrote the book, "Modern Technical Writing" whose principles were used in this guide.




### Frequently Asked Questions 
1. ##### Q: Why is markdown better than using a word processor? 

	A: One of the principles from Andrew Etter's book is to use a lightweight markup language. Markdown is the easiest markup language to learn for a beginner compared to HTML and XML. Aside from that, documents produced using word processors (e.g. .docx and .pdf files) are very incompatible with website hosting. Furthermore, it is better to use distributed version control for long-term technical documentation. This is because it saves the file online and can thus, be easily retrieved.
	
	
2. ##### Q: Why is my Resume not showing up? 

	A: There are a couple of reasons why your resume might not show up. The first step would be to check that your repository is correctly named using the format: `username.github.io`. If that is correct, and you still cannot see your resume, check that the file is correctly named `index.md.` Note that for GitHub file names, the case is important as `Index.md` is different from `index.md.`
	
	
