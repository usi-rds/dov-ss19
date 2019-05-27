# GitHub Classroom configuration tutorial
If you're reading this, hopefully, you've accepted your invitation to the GitHub Classroom using the link [classroom.github.com/a/TBD](https://classroom.github.com/a/TBD), and you're viewing your private repository.
Congratulations, you're halfway through the initial setup procedure!

With GitHub Classroom, you have your private copy (a.k.a. fork) of the teacher's repository. Nothing that your change in your private repository affect's the teacher's or other student's repositories. However, you want to be able to get any changes made by the teacher through the course.

With the following step's, you'll set up your local repository on your machine in a way that you can pull (keep up to date) any changes the teacher has made using one simple command.

## Prerequisites
- Make sure you have installed Git on your machine,
- you've enrolled to the class,
- cloned your private fork to your machine and
- you have received and accepted your invitation to collaborate on the the master repository ([https://github.com/usi-rds/dov-ss19](https://github.com/usi-rds/dov-ss19))

> It might take up to a few hours to receive your collaboration invitation email after you've enrolled in GitHub to the class. If you still don't receive your invitation email after 24 hours, please reach out to summerschooldov@usi.ch.

## Configuration steps
a. Open Terminal (Linux or Mac) or Git Bash (Windows)

b. Change the current working directory to your local project.

```
cd ~/dov-ss19-YOUR_GITBHUB_PRIVATE_REPOSITORY
```

c. Add a new remote called upstream that point's to the teacher's master repository

```
git remote add upstream git@github.com:usi-rds/dov-ss19.git
```

## Sync workflow
Whenever you want to get the latest changes from the teacher's repository, you only need to execute
```
git pull upstream master
```
from your local project's directory. This will get the latest changes from the teacher's repository and merge it into your local master branch.
