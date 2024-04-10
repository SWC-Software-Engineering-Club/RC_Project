# SWC Software Engineering Club

## RC Self-driving Car Project

Our project aims to immerse ourselves in the realm of AI/ML by applying these cutting-edge technologies to a tangible real-world application: building a self-driving RC car. Through this endeavor, we aspire to gain valuable experience across multiple domains, including hardware integration, software development, and ML algorithm implementation. By embracing in-demand concepts such as deep learning, we strive to deepen our understanding and proficiency in these transformative technologies.

Beyond technical skills, our project offers an opportunity to hone essential soft skills such as collaboration and leadership within a team setting. Through collaborative efforts, we aim to leverage each team member's strengths to overcome challenges and achieve our shared goal of successfully completing the RC project. This endeavor serves as a platform for us to take initiative, demonstrate leadership, and cultivate expertise in the rapidly evolving field of ML.

## Git

### What Is Git?

• Open-source version control system that manages changes to files
and other data.

• Not to be confused with GitHub. GitHub is an Internet hosting service
for software development and version control using Git.

### Common Git Commands

• Clone: Bring a repository hosted somewhere like Github into a folder
in your computer.

• Add: Track your files and changes of a file in Git.

• Commit: Save your files to Git.

• Push. Upload Git commits to a remote repository, like Github.

• Pull. Download changes from remote repo to your local computer.

### Getting Started

**Clone Repository**

Using git clone, clone the remote repository into your computer.

```console
git clone <repository URL>
```

**Add Files**

Once you begin working on the project and start to add your own files or work to it, you can stage your changes by using add. You can add individual files with:

```console
git add <filename>
```

You can also add all the files at once instead of adding them individually by typing:

```console
git add .
```

You can then use:

```console
git status
```

to see all the files that are staged after using add.

**Commit Your Changes**

You can now save changes made to the files that you added before. Commiting changes allows you add a message describing the modifications made.

```console
git commit -m "<message with info about changes>"
```

**Push to GitHub Repo**

Now you can push the changes to the online repository.

```console
git push origin <branch name>
```

Example:

```console
git push origin main
```

**Pulling**

• After a pull request passes and everything is merged it’s a good idea
pull all the new information into your local repository with:

```console
git pull origin main
```

### Branching

• We use branches to be able to work in a particular instance of the
main branch in order to prevent disruptions on your main branch, and
also to not create conflicts with your teammates work.

• You can check which branch you are currently on with:

```console
git branch
```

**Create a Branch**
• To create a branch we use the checkout command, we also use it to
be switching between branches

• To create a branch use the following:

```console
git checkout -b nameofbranch
```

• To switch between branches:

```console
git checkout nameofbranch
```

## Setting up a Virtual Environment

A virtual environment is essential for Python projects to maintain dependencies and ensure consistency across different projects. It isolates project-specific packages from the global Python environment, preventing conflicts between different projects.

### Why Use a Virtual Environment?

1. **Dependency Isolation**: Different projects may require different versions of the same package. A virtual environment allows you to install project-specific dependencies without affecting other projects.

2. **Reproducibility**: By encapsulating dependencies within a virtual environment, you can ensure that anyone who runs your project gets the same environment, reducing compatibility issues and ensuring reproducibility.

3. **Security**: Using a virtual environment helps mitigate security risks by sandboxing project dependencies. It prevents unintended modifications to system-wide packages and potential security vulnerabilities.

### How to Set Up a Virtual Environment

To set up a virtual environment for your Python project, follow these steps:

```console
$ python -m venv venv
```

This command creates a new virtual environment named 'venv' in the current directory.

### Activating the Virtual Environment

After creating the virtual environment, you need to activate it before working on your project. Use the following command:

#### For Windows:

```console
$ venv\Scripts\activate
```

### For macOS/Linux:

```console
$ source venv/bin/activate
```

Once activated, you'll see the name of the virtual environment in your command prompt, indicating that you're now working within the virtual environment.

Remember to activate the virtual environment every time you start working on your project to ensure that you're using the correct dependencies.

## Managing Project Dependencies with requirements.txt

The `requirements.txt` file is commonly used in Python projects to specify the dependencies required for the project to run. It lists all the Python packages along with their versions that are necessary for the project.

### Importance of requirements.txt

1. **Reproducibility**: The `requirements.txt` file ensures that everyone working on the project can easily install the same set of dependencies, leading to consistent environments across different systems.

2. **Dependency Management**: It simplifies dependency management by providing a centralized location to track and manage project dependencies.

### Installing Packages from requirements.txt

To install the packages listed in the `requirements.txt` file, you can use the following command:

```console
$ pip install -r requirements.txt
```

This command reads the requirements.txt file and installs all the listed packages along with their specified versions.

### Adding Packages to requirements.txt

If you need to add new packages to the project, you can do so by installing the packages using pip and then updating the requirements.txt file. Here's how you can add a package to requirements.txt:

Install the package using pip:

```console
$ pip install <package-name>
```

After installing the package, update the `requirements.txt` file to include the new package and its version:

```console
$ pip freeze > requirements.txt
```

By maintaining an up-to-date requirements.txt file, you ensure that all project collaborators can easily replicate the project environment and dependencies.
