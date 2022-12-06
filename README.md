# Capstone Project (Cloud DevOps Engineer)

Capstone project for Udacity Dev-Ops Nanodegree: develop a CI/CD pipeline for micro services applications with either blue/green deployment or rolling deployment.

## CI CD Pipeline

The CI CD pipeline is as follows for this project. For initial set up:

- Set up CircleCI
- Install dependencies for local development
- Create AWS infrastructure

For application development:

- Make development change
- setup CircleCI
- Commit to git
- Push to repository

## Running the stuff

There is a `Makefile` that contains lots of useful commands.
Running `make` will list them, like the below output.

```text
setup:          Create the virtial environment to run this project
install:        Install the required imports for this project
test:           Run the tests for this prject
lint:           Check the validity of the project files
```


## CircleCI setup

Link CircleCI to project github
Add Enviroment on CircleCI 

## Output

From running the above the following will be created.

CIRCLECI FLOW:
![Full pipline pass](./img/Screenshot-stages-pipline-pass.png)

CircleCI build when the lint fails:
![lint failing](./img/Screenshot-fail-make-lint.png)

CircleCI build when the lint pass:
![lint pass](./img/Screenshot-make-lint-pass.png)

Step build docker success
![Screenshot build docker success](./img/Screenshot-build-docker-success.png)

Step push image to docker hub:
![Screenshot-push-docker-to-docker-hub](./img/Screenshot-push-docker-to-docker-hub.png)

Build stack on Cloudformation:
![Screenshot-cloudformation-create](./img/Screenshot-cloudformation-create.png)

Create EC2 Success:
![Screenshot-ec2-runing](./img/Screenshot-ec2-runing.png)

Create EKS Success:
![Application running in AWS](./img/Screenshot-eks-deloy.png)

<h3>Author</h3>
<a href = "https://github.com/dainh222/Udacity-AWS-DevOps-Engineer-Capstone-Project-5">GitHub</a>
