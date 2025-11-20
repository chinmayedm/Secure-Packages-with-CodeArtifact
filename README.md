# Secure Packages with CodeArtifact
![codeartifact](https://github.com/chinmayedm/Secure-Packages-with-CodeArtifact/blob/main/Screenshot%202025-11-20%20at%2010.42.14.png?raw=true)

# What is AWS CodeArtifact?

AWS CodeArtifact is a managed repository service for storing and managing software packages.
It helps with dependency management and integrates seamlessly with other AWS services.

# How I Used CodeArtifact in This Project

I used AWS CodeArtifact in today’s project to store and manage dependencies, enabling seamless access to required packages and ensuring consistent builds across environments.

# One Thing I Didn’t Expect

One thing I didn’t expect was the level of integration required between services like CodeArtifact, IAM, and CodePipeline to automate the build and deployment process.

# My Project Has Three Artifact Repositories
# Local Repository

The local repository is a personal toolbox where we keep all the tools and materials for the current project.

# Upstream Repository

The upstream repository is the original or main repository from which a forked repository derives.
It serves as the primary source of code updates and allows developers to sync their fork with the latest changes.

# Public Repository

The public repository is a Git repository accessible to anyone on platforms like GitHub.
It allows open-source collaboration where users can clone, fork, and contribute to the project while maintaining transparency and accessibility.
![Repositories](https://github.com/chinmayedm/Secure-Packages-with-CodeArtifact/blob/main/Screenshot%202025-11-20%20at%2010.43.07.png?raw=true)

# Connecting My Project With CodeArtifact

I connected my web app project to CodeArtifact to securely manage dependencies, streamline package versioning, and ensure seamless integration with AWS services.
This improved build consistency, reduced security risks, and optimized deployment workflows.

# Creating settings.xml

I created a new file called settings.xml in my web app.

settings.xml is a Maven configuration file that manages repositories, authentication, proxies, and build settings for dependency resolution and secure access.

The snippets in settings.xml configure authentication for AWS CodeArtifact, define repository access, and manage dependency resolution.
They include:

1. server credentials

2. repository URLs

3. permissions for secure and efficient package retrieval
![settings.xml]()

# Testing the Connection

To test the connection between Cloud9 and CodeArtifact, I compiled my web app.

# Compilation

Compiling means converting source code into machine code or bytecode that can be executed by a computer.

# Success

After compiling, I checked the local project directory and the GitHub repository.
The project was up to date with the latest changes, and there were no issues or errors related to the compiled code.
![Testing]()

# Creating IAM Policies
# Importance of IAM Policies

I created an IAM policy because it allows me to define and manage specific permissions for users or services within AWS.
This ensures they have appropriate access to resources like CodeArtifact, EC2, or S3 while maintaining security and control.

# My IAM Policy

I defined my IAM policy using JSON.
This policy allows access to AWS CodeArtifact, including retrieving and publishing packages.
![IAM policies]()
