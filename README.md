
# P3 - Dependencies and CodeArtifact


**Author:** Aleemuddin Mohammad  
**Email:** aleemuddin.work@gmail.com

---

## Store Dependencies with CodeArtifact

![Image](http://learn.nextwork.org/surprised_black_smart_goose/uploads/aws-devops-code-artifact_1d79e699)

---

## Introducing today's project!

### What is AWS CodeArtifact?

AWS CodeArtifact is a managed artifact repository service that helps securely store and share software packages within your development workflows. It integrates well with build tools, enhancing both security and scalability.

### How I used CodeArtifact in this project

In today's project, I used AWS CodeArtifact to manage and secure the dependencies required by our application. By connecting our development environment to CodeArtifact, we ensured that all team members accessed the same set of approved, secure libra

### One thing I didn't expect in this project was...

One thing I didn’t expect in this project was the complexity of configuring AWS CodeArtifact with our existing development tools. The integration required careful adjustments to ensure compatibility and smooth functioning between different systems.

### This project took me...

This little project took me les than 30 minutes. 

---

### My project has three artifact repositories

The local repository is the personal toolbox where you keep all the specific tools and materials for your current project.

The upstream repository is the point to the big library, helping us get and store new tools when we need them for our toolbox.

The public repository is ther vast package library on the internet where all sorts of tools and materials are stored. It's the primary source that supplies packages to other applications. 

![Image](http://learn.nextwork.org/surprised_black_smart_goose/uploads/aws-devops-code-artifact_ef93d32c)

---

## Connecting my project with CodeArtifact

I connected my web app project via my VScode IDE to CodeArtifact to manage dependencies securely and efficiently across my AWS environments.

### I created a new file, settings.xml, in my web app

settings.xml is a configuration file for Maven that customizes build settings, including repositories, proxy specifications, and server credentials for project builds.

The snippets of code in the `settings.xml` file define custom configurations for Maven projects. These include specifying alternative locations for local repositories, configuring remote repository access, and managing credentials.

![Image](http://learn.nextwork.org/surprised_black_smart_goose/uploads/aws-devops-code-artifact_c17eace8)

---

## Testing the connection

### To test the connection between Cloud9 and CodeArtifact, I compiled my web app

Compiling is like translating your project’s code into a language that computers can understand and run. When you compile your project, you're making sure everything is correctly set up and ready to turn into a working app.

### Success!

After compiling, I checked java-app-packages repository where I found package names and their details. 

![Image](http://learn.nextwork.org/surprised_black_smart_goose/uploads/aws-devops-code-artifact_1d79e699)

---

## Create IAM policies

### The importance of IAM policies

I also created an IAM policy I also created an IAM policy because

### I defined my IAM policy using JSON

This policy will give a service temporary security credentials to interact with CodeArtifact. AWS services will then use the credentials to request an authorization token (which is the GetAuthorizationToken action you've allowed) that lets them acce

![Image](http://learn.nextwork.org/surprised_black_smart_goose/uploads/aws-devops-code-artifact_9b2ded4f)

---

---
