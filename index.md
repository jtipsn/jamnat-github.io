# Git and GitHub Activity: Pushing Your First Change

Welcome to the Git and GitHub hands-on activity! Follow the steps below to push your first change to a GitHub repository.

---

## Step 1: Set Up Your Environment

### 1.1 Create a GitHub Account
- Visit [GitHub.com](https://github.com) and sign up using your UoA email if you haven't already.
- Skip the setup steps for now—just create your account.

### 1.2 Install Git on Your Computer
- Go to [Git's download page](https://git-scm.com/downloads) and download the installer for your operating system.
- Follow the installation instructions, and select the default options during setup.
- Open your terminal or Git Bash and run the following commands to configure Git with your email and GitHub username:
<pre><code>git config --global user.email "&lt;email&gt;"</code></pre>
<pre><code>git config --global user.name "&lt;username&gt;"</code></pre>


---

## Step 2: Clone the Repository

### 2.1 Create a Directory for Your Project
1. Open **Git Bash** (or your terminal) on your computer.
2. Navigate to where you want to create your project folder using the `cd` command:
 
   <pre><code> cd <path-to-your-folder></code></pre>

4. Create a new directory for your project:
mkdir my-first-repo cd my-first-repo

### 2.2 Create a new repository in Github
<img width="328" alt="image" src="https://github.com/user-attachments/assets/43ee4436-0591-4769-afee-7e325c561ae4" />

In the Github webpage click new and create a name for your repository and add a README and create:
This will take you your repository page.

Now, you'll clone the GitHub repository to your local machine:
1. Copy the **URL** of the repository (Click on the green "Code" button and then copy the URL under `HTTPS`).<img width="688" alt="image" src="https://github.com/user-attachments/assets/a03c1110-a642-4fdb-a58e-e75a027a4161" />

3. In your terminal, run the following command, replacing `<repo-url>` with the copied URL:
<code><pre>git clone <repo-url></code></pre>
which will create a folder with the repo name. Then run `cd <repo_name>` to go to the working directory
 
---

## Step 3: Make Changes to Your Files

### 3.1 Create a New File
1. Create a new file inside your repository directory. For example, to create a file named `<student_name>_first_commit.txt`, run:
 
   <code><pre>echo "Hello, Git!" > <student_name>_first_commit.txt</code></pre>
Alternatively, you can create and edit the file using any text editor, and save it in the project directory. The key is that the file should be added to the Git repository folder.

Once the file is created, you can run the ls or dir command to list the files in your current directory and verify that the new file has been added:


---

## Step 4: Add Your Changes

### 4.1 Add Files to the Staging Area
To track the changes you've made, use the `git add` command:
- Add the specific file:
git add <student_name>_first_commit.txt.  You could also use `git add .` to add all changed files

Then run `git status` in the terminal to see what has been modified or added

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
When pushing, a broswer prompt will pop up asking for a login.  Once you authenticate, the commit will be get pushed to the github repo

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
