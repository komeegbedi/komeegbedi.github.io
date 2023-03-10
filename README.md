# How To Host Your Resume Using Markdown , VS Code, GitHub Pages and Jekyll.


### Step 1: Download and Install Visual Studio Code (VS Code):

VS Code is a free code editor. It comes with built-in support for different programming and markup languages including Markdown.

1. If you don't already have VS Code installed, you can download by going to [VS Code website](https://code.visualstudio.com/).
2. Download and install VS Code for your operating system.


### Step 2: Create a GitHub Pages repository

GitHub is  a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere. Github Pages helps you turn your Github repository into websites.

1. If you don't already have a GitHub account, create one by going to [github.com](github.com) and following the sign-up instructions.
2. Create a new repository by clicking the green "New" button located at the top left of the main page of your GitHub account.
3. Name the repository `yourusername.github.io` and make sure it is set to public. where _yourusername_ is your username on GitHub. If the first part of the repository doesn’t exactly match your username, it won’t work, so make sure to get it right.
4. Click on the "Create repository" button.

### Step 3: Clone the repository to your local machine

1.  First, you'll need to install Git on your computer. You can download it from the official website: [https://git-scm.com/downloads](https://git-scm.com/downloads). Follow the prompts to install Git on your computer.
    
2.  Once you have Git installed, open your command line interface. On Windows, this is called the "Command Prompt," and on Mac/Linux, it's called the "Terminal."
    
3.  Navigate to the directory where you want to clone the repository. You can do this by typing `cd` followed by the path to the directory. For example, if you want to clone the repository to your desktop, you can type:

	   `cd ~/Desktop`

5.  Now, you will need the URL of the repository you want to clone. You can find this by going to the repository's homepage and clicking the "Code" button, you will see 3 tabs, under the "HTTPS" tab you should see the URL of the repository.
    
6.  Once you have the URL, go back to your command line and type the following command, replacing `URL` with the actual URL of the repository:

	`git clone URL` 

### Step 4: Create a new file in VS Code and format your resume in Markdown 

 1.  After installing VS Code, create a new folder on your computer to store your resume project.  
 2.  Open Visual Studio Code and click "File" > "Open Folder", then navigate to the folder of the clone repository and click "Open".  
 3.   In Visual Studio Code, click "File" > "New File" and name the file "index.md" (or any name you prefer but be sure the file extension is ".md") . This is where you'll write your resume content in Markdown format.
 4.  Open the "index.md" file and start writing your resume content using Markdown syntax. To learn more about Markdown syntax visit  [HERE](https://www.markdowntutorial.com/) 
 5. You can also download an extension in VS Code to help you preview your markdown files while you are writing. The extension name of the extension I used is "Markdown All in One". 

### Step 5: Create a Static Website with Jekyll 

  Jekyll is a static site generator. It takes text written in your favourite markup language and uses layouts to create a static website. To customize the look of your resume, we are going to use a Jekyll theme.

The Jekyll resume theme we will be using can be found [https://github.com/sharu725/online-cv](https://github.com/sharu725/online-cv) but you can find more themes by visiting [https://jekyllthemes.io/](https://jekyllthemes.io/)

  1. Before you can use Jekyll, you will need to install it on your computer.  You can follow the [Guides on Jekyll website for the installation process](https://jekyllrb.com/docs/installation/).
  
  2. We will need to clone the repository of the Jekyll theme template we are using into our project on our local machine. Run the following command in your terminal:
  
		`git clone https://github.com/sharu725/online-cv.git`
3.  Next we need to install the required ruby gems.

	`bundle install`
	
4. Next, we Build the site and make it available on a local computer.
	`bundle exec jekyll serve`
	
	If this step fails. run this command first 
	
	`bundle add webrick` 
	then try running the previous command again. 
	
5. Now, it's time to preview your site locally. To preview your site locally. Open your browser and navigate to `http://localhost:4000`
	
6. To modify the descriptions on the website, you can do that from the `_config.yml` file.
  
### Step 5: Push your files to GitHub

There are two ways to push your files to GitHub. You can do it either directly from VS Code or from the command prompt. 

To push your files directly from VS Code:
1.  In VS Code, click on the source control icon on the left-hand side of the screen.

2.  Click on the "+" icon to stage all changes.

3.  After staging your changes, enter a commit message describing the changes and click on the checkmark to commit your changes.

4.  Click on the ellipsis (...) icon and select "Push".

To push your files through the Command Prompt: 

1.  In your terminal, navigate to the repository folder and run the command `git add .` to stage all changes.
    
2.  After staging your changes, commit them with a message describing the changes using the command `git commit -m "commit message"`.
    
3.  Finally, push your changes to the remote repository on GitHub with the command `git push`.
    
4.  If this is your first time pushing changes to GitHub from this computer, you may be prompted to authenticate. Follow the prompts to authenticate with your GitHub username and password.

  Congratulations! You have successfully hosted and formatted your resume using Markdown, VS Code, GitHub Pages, and Jekyll. You should have something looking like this now: 


## More Resources
 
1. [Markdown Tutorial](https://www.markdowntutorial.com/) 
2. [Andrew Etter's book Modern Technical Writing](https://a.co/d/4H7ERuI)
3. [Git](https://www.w3schools.com/git/)

 ## Authors and Acknowledgements 
 
1. Jekyll Resume Template -  Sharath Kumar (-   [https://webjeda.com](https://webjeda.com/)

2. Group Members - Khanh Le,  Zhiyin An and Christian Trites 

## FAQ

#### Why is Markdown better than a word processor?

Markdown is a lightweight markup language that is easy to learn and use. It allows you to focus on the content of your document without worrying about formatting. Markdown documents can be easily converted