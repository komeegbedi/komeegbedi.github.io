# How To Host Your Resume On GitHub Pages

**Step 1: Create a GitHub Account** If you don't already have a GitHub account, create one by going to github.com and following the sign-up instructions.

**Step 2: Create a New Repository** Click the "+" button on the top right corner of your GitHub homepage and select "New Repository". Give your repository a name (for example, "resume") and make sure to keep it public.

**Step 3: Clone Your Repository** To clone your repository, you will need to use Git. Open your terminal and type:

    git clone https://github.com/yourusername/resume.git
    
Replace "yourusername" with your actual GitHub username and "resume" with the name of your repository.

**Step 4: Install Jekyll** Before you can use Jekyll, you will need to install it on your computer. Follow the instructions on the Jekyll website to install it on your operating system.

**Step 5: Create a New Jekyll Site** Open your terminal and navigate to your resume repository by typing:

    cd resume
Then, create a new Jekyll site by typing:

    jekyll new .

This will create a new Jekyll site in your current directory.

**Step 6: Edit Your Resume** Open the index.md file located in the root directory of your resume repository. This is where you will write your resume using Markdown syntax.

**Step 7: Preview Your Site Locally** To preview your site locally, run the following command in your terminal:

    bundle exec jekyll serve
Then, open your web browser and navigate to [http://localhost:4000](http://localhost:4000/). You should be able to see your site and any changes you make to the index.md file will be automatically updated.

**Step 8: Commit and Push Your Changes** Once you are happy with your resume, it's time to commit and push your changes to GitHub. To do this, run the following commands in your terminal:

    git add .
    git commit -m "Added my resume"
    git push origin main

This will add your changes to the staging area, commit them with a message, and push them to the "main" branch of your repository on GitHub.

**Step 9: Enable GitHub Pages** Finally, to enable GitHub Pages, go to your repository settings and scroll down to the "GitHub Pages" section. Select "main" as your branch and "/" as your root directory, then click "Save". Your resume should now be live at [https://yourusername.github.io/resume/](https://yourusername.github.io/resume/).



[link to template used](https://github.com/sharu725/online-cv)