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
