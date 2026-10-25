Assignment 1.5 — GitHub Essentials II

Aim

To upload a local project to GitHub and learn how to push commits to a remote repository.

Procedure

1. Created a GitHub account or signed in to an existing account.
2. Created a new public repository on GitHub.
3. Connected the local Git repository to the remote GitHub repository.
4. Uploaded project files using the "git push" command.
5. Created a new file and committed the changes.
6. Pushed the second commit to GitHub.
7. Verified the commit history on GitHub.

Terminal Commands

1. Configure Git

git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

2. Create a Local Project

mkdir github-practice
cd github-practice
git init

Create a file named "index.html" with the following code:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Practice</title>
</head>
<body>
    <h1>My First GitHub Project</h1>
    <p>Learning Git and GitHub.</p>
</body>
</html>

3. Create the First Commit

git add index.html
git commit -m "Add initial HTML page"

4. Create a Public GitHub Repository

1. Visit https://github.com/
2. Sign in to your account.
3. Click the New repository option.
4. Enter the repository name as "github-practice".
5. Select Public.
6. Click Create repository.

5. Connect the Local Repository to GitHub

Replace "YOUR-USERNAME" with your actual GitHub username.

git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/github-practice.git
git push -u origin main

6. Add a New File and Create the Second Commit

Create a file named "about.html" and add the following code:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About My Project</title>
</head>
<body>
    <h1>About My Project</h1>
    <p>This project helps me practice Git and GitHub.</p>
</body>
</html>

Run the following commands:

git add about.html
git commit -m "Add project information page"
git push origin main

7. Verify the Commit History

git log --oneline

Open your GitHub repository in the browser and check the Commits section to verify that both commits are available.

Expected Output

1. A public GitHub repository is created successfully.
2. The local project is connected to the remote repository.
3. The "index.html" file is uploaded to GitHub.
4. The new "about.html" file is added and pushed successfully.
5. Both commits appear in the GitHub commit history.

Observations

1. GitHub hosts Git repositories online.
2. The "git remote add" command connects a local repository to a remote repository.
3. The "git push" command uploads local commits to GitHub.
4. Each commit records a snapshot of project changes.
5. GitHub displays repository files and commit history.

Result

The local project was uploaded to a public GitHub repository successfully. A second file was added, committed, and pushed, and the commit history was verified.

Submission

Public GitHub Repository Link:

https://github.com/YOUR-USERNAME/github-practice

Replace "YOUR-USERNAME" with your actual GitHub username and submit the working public repository link.
