# Git and GitHub Activity: Pushing Your First Change

Welcome to the Git and GitHub hands-on activity! Follow the steps below to push your first change to a GitHub repository.

---

## Step 1: Set Up Your Environment

### 1.1 Create a GitHub Account
- Visit [GitHub.com](https://github.com) - use your UoA email to sign up if you haven't already.  When signing up skip all the set up for now.   

### 1.2 Install Git on Your Computer
- Go to [Git's download page](https://git-scm.com/downloads) and download the version for your operating system: Windows or Mac.
- Follow the installation instructions.  Choose the default options on everything!

---

## Step 2: Clone the Repository

### 2.1 Create a Directory for Your Project
1. Find and Open the App `Git bash` in the windows search bar
2. Navigate to where you want to create your project folder using the
3. `cd` command: cd <path-to-your-folder> git bash by default goes to the user profile.  

4. Create a new directory for your project:
mkdir my-first-repo cd my-first-repo

### 2.2 Clone the Repository from GitHub
Now, you'll clone the GitHub repository to your local machine:
1. Go to https://github.com/jtipsn/git-session.git
2. Copy the **URL** of the repository (Click on the green "Code" button and then copy the URL).<img width="688" alt="image" src="https://github.com/user-attachments/assets/a03c1110-a642-4fdb-a58e-e75a027a4161" />

3. In your terminal, run the following command, replacing `<repo-url>` with the copied URL:
`git clone  https://github.com/jtipsn/git-session.git` to download to repo to your local environment and `cd git-session` to go to the working directory
 
---

## Step 3: Make Changes to Your Files

### 3.1 Create a New File
1. Create a new file in the repository. For example, you can create a `<student_name>_first_commit.txt` file:
echo "Hello, Git!" > <student_name>_first_commit.txt

 

### 3.2 Check the Status of Your Repository
Before committing your changes, check the status of your repository to see which files have been modified or added:
git status

---

## Step 4: Add Your Changes

### 4.1 Add Files to the Staging Area
To track the changes you've made, use the `git add` command:
- Add the specific file:
git add <student_name>_first_commit.txt

- Or add all modified/created files:
git add .
 

---

## Step 5: Commit Your Changes

### 5.1 Commit with a Message
Now, commit your changes to the local repository:
git commit -m "Add <student_name>_first_commit.txt with a greeting message"

- The message inside the quotes (`"Add <student_name>_first_commit.txt with a greeting message"`) should describe what you've changed.

---

## Step 6: Push Your Changes to GitHub

### 6.1 Push to GitHub
Push your local commits to the GitHub repository:
git push origin main


- `origin` refers to your GitHub repository.
- `main` is the default branch name (if your repository uses `master` instead of `main`, use `master`).

---

## Step 7: Verify the Changes on GitHub

1. Go to your GitHub repository in your web browser.
2. You should see the `<student_name>_first_commit` file in your repository with the changes you just made.

---

### Congratulations! 🎉
You’ve successfully pushed your first change to GitHub!

Keep experimenting with Git by making more changes, creating branches, and collaborating with others!

---

## Helpful Git Commands

Here’s a list of some common Git commands:

- `git status` – Check the status of your repository (see changes).
- `git add .` – Stage all changes.
- `git commit -m "message"` – Commit your changes with a message.
- `git push origin main` – Push changes to the remote repository (GitHub).
- `git pull origin main` – Pull the latest changes from the remote repository.
- `git clone <repo-url>` – Clone a repository from GitHub to your local machine.

If you need help, feel free to ask questions!
