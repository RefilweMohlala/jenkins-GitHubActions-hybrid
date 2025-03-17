# jenkins-GitHubActions-hybrid
Flask CI/CD Hybrid Pipeline Using Jenkins and GitHub Actions

# Jenkins and GitHub Actions Hybrid CI/CD Pipeline

This repository demonstrates a hybrid Continuous Integration (CI) and Continuous Deployment (CD) pipeline, utilizing both **GitHub Actions** and **Jenkins** to automate testing for a Python Flask application. The hybrid approach ensures a smooth and redundant process for continuous testing, combining the best features of both platforms.

## Overview

In this project, we set up two CI/CD tools—**GitHub Actions** and **Jenkins**—to create a pipeline that automatically tests our Flask application on every push to the `main` branch or when pull requests are made. This approach allows for flexibility, redundancy, and effective testing of the application.

### How the Pipeline Works

1. **GitHub Actions**: This CI tool is set up to run tests whenever changes are pushed to the `main` branch or a pull request is made. It sets up the environment, installs dependencies, and runs tests automatically as part of the CI process.
   
2. **Jenkins**: Jenkins is integrated into the process to offer additional build and test capabilities, with the flexibility to manually trigger builds. It helps ensure that all aspects of the application are continuously tested in a consistent environment.

By combining these two tools, we ensure that the application is tested continuously in multiple environments, with both tools performing similar tasks in parallel. This gives us an extra layer of confidence in the stability of the code.

## Technologies Used

- **Flask**: For building the web application.
- **GitHub Actions**: For automated CI with testing.
- **Jenkins**: For additional CI automation with the ability to trigger builds manually.
- **Python 3.9**: As the runtime environment for testing the application.
- **pytest**: For running unit tests on the Flask application.

## Features

- **Automatic Testing with GitHub Actions**: Whenever a change is pushed to the `main` branch or a pull request is created, the pipeline automatically runs, setting up the environment, installing dependencies, and executing the tests.
  
- **Redundancy with Jenkins**: Jenkins offers another layer of testing, which can be manually triggered for builds and tests. This ensures additional flexibility and control over the CI/CD pipeline.

- **Easy Integration**: Both CI tools are configured to work independently yet together, ensuring seamless testing and continuous feedback on the application’s health.

## Workflow

1. **GitHub Actions** is triggered by pushes or pull requests to the `main` branch.
2. It runs a set of steps to set up a virtual environment, install dependencies, and run tests using **pytest**.
3. **Jenkins** can be triggered manually to run the same tests, allowing you to validate the functionality of the application within the Jenkins environment as well.

## How to Test the Pipeline

- **For GitHub Actions**: Simply push changes to the `main` branch or open a pull request. This will trigger the GitHub Actions workflow to run the tests.
  
- **For Jenkins**: Jenkins is configured to run manually. You can trigger Jenkins builds when needed, ensuring the application runs in a controlled, consistent environment.

## Screenshots
Webhook
![webhooks](https://github.com/user-attachments/assets/22d5dc2a-5c50-4be4-8a56-599054d9d9a0)
Jenkins build success
![Jenkins build success](https://github.com/user-attachments/assets/54a118e1-d548-486a-8d00-c060e5d4171a)
Jenkins console output
![Jenkins console output](https://github.com/user-attachments/assets/3fd27354-af62-4768-8347-92defb1bcdaf)
Github actions build success
![Github build success](https://github.com/user-attachments/assets/8f3efb5d-3d9e-40c3-9231-ef8ee77562a2)
Github Actions workflow
![github actions workflow](https://github.com/user-attachments/assets/18f9f2fa-b261-4737-a876-e981a1a1c0e2)


## Conclusion

This hybrid setup with GitHub Actions and Jenkins allows you to enjoy the advantages of both platforms. **GitHub Actions** provides seamless automation for continuous testing and deployment, while **Jenkins** offers flexibility for more complex workflows, manual triggers, and additional control over your CI/CD pipeline.

Feel free to modify the pipeline configuration to suit your needs or expand it further to include deployment steps, notifications, or additional tests.
