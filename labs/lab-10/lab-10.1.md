# Lab 10.1: Creating a GitHub Page to Showcase Your Profile and Skills
By the end of this exercise, you will have created a personal GitHub Pages site to promote your profile, projects, and skills.
### Step 1: Create a New Repository
1.	Log in to GitHub: Go to GitHub and log in to your account.
2.	Create a Repository:
    -	Click on the + icon in the top right corner and select New repository.
    -	Name the repository <username>.github.io, where <username> is your GitHub username.
    -	Set the repository to Public.
    -	Optionally, add a description.
    -	Click Create repository.
### Step 2: Clone the Repository
1.	Open Terminal or Command Prompt: Open your terminal (Mac/Linux) or Command Prompt (Windows).
2.	Clone the Repository:
     -	Run the following command to clone the repository to your local machine:
      ```bash
      git clone https://github.com/<username>/<username>.github.io.git
      ```
     -	Replace `<username>` with your GitHub username.
### Step 3: Create Your Website
1.	Navigate to the Repository:
    -	Change directory to your repository:
    ```bash
    cd <username>.github.io
    ```
2.	Create an Index File:
    -	Create an index.html file:
    ```bash
    touch index.html
    ```
    -	Open index.html in your preferred text editor and add the following basic HTML structure:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>My GitHub Page</title>
    </head>
    <body>
        <h1>Welcome to My GitHub Page</h1>
        <p>This is my personal website where I highlight my projects and skills.</p>
    </body>
    </html>
    ```
### Step 4: Customize Your Site (Optional)
1.	Add Content: 
    -	Customize the index.html file to include sections like About Me, Projects, and Contact.
    -	Use Markdown or HTML to format your content.
2.	Add Styles: 
    -	Create a styles.css file to add custom styles to your site.
    -	Link the CSS file in your index.html:
    ```html
    <link rel="stylesheet" href="styles.css">
    ```
### Step 5: Commit and Push Changes
1.	Add Changes: 
    -	Stage your changes:
    ```bash
    git add .
    ```
2.	Commit Changes: 
    -	Commit your changes with a message:
    ```bash
    git commit -m "Initial commit"
    ```
3.	Push Changes: 
    -	Push your changes to GitHub:
    ```bash
    git push origin main
    ```
### Step 6: Enable GitHub Pages
1.	Go to Repository Settings: 
    -	Navigate to your repository on GitHub.
    -	Click on Settings.
2.	Enable GitHub Pages: 
    -	Scroll down to the GitHub Pages section.
    -	Under Source, select main branch.
    -	Click Save.
### Step 7: View Your Site
1.	Access Your Site: 
    -	Your site should now be live at https://<username>.github.io.
    -	Open this URL in your web browser to view your site.
### Step 8: Continuous Improvement
1.	Update Regularly: 
    -	Regularly update your site with new projects, blog posts, and other content.
2.	Seek Feedback: 
    -	Ask peers and mentors for feedback to continuously improve your site.
 
Congratulations! You have successfully created a GitHub Pages site, a straightforward way to promote yourself online. Keep refining and updating your site to reflect your latest work and achievements.
