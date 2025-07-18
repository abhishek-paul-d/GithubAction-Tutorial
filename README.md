# GithubAction-Tutorial

## Continuous Integration (CI) and Continuous Deployment (CD)

Continuous Integration (CI) and Continuous Deployment (CD) are important software development practices that help automate the build, test, and deployment processes.

Continuous Integration (CI) is the practice of regularly merging code changes into a shared repository, and then automatically building and testing the application to detect integration issues early. This ensures that new code changes don't break existing functionality.

Continuous Deployment (CD) is the practice of automatically deploying the application to a production environment after the CI process passes. This allows for faster feedback and iteration on the codebase, as changes can be delivered to users more frequently.

## GitHub Actions

GitHub Actions is a powerful tool that enables the implementation of CI and CD workflows directly within a GitHub repository. It provides a wide range of pre-built actions and the ability to create custom actions, allowing developers to automate various software development tasks.

## This Project

This is a sample project that demonstrates the usage of GitHub Actions for Continuous Integration and Continuous Deployment.

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/abhishek-paul-d/GithubAction-Tutorial.git
   ```
2. Change to the project directory:
   ```
   cd GithubAction-Tutorial
   ```
3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

### Usage

1. Run the math operations:
   ```
   python src/math_operations.py
   ```
2. Run the unit tests:
   ```
   python -m unittest discover tests
   ```

### CI/CD Workflows

This project uses the following GitHub Actions workflows to implement Continuous Integration and Continuous Deployment:

#### Continuous Integration (CI)

The `unittest.yml` workflow runs the unit tests on every push and pull request to the repository. This ensures that new code changes don't break existing functionality.

The workflow performs the following steps:
1. Checkout the code
2. Set up the Python environment
3. Install the project dependencies
4. Run the unit tests using the `python -m unittest discover tests` command

#### Continuous Deployment (CD)

The `python-app.yml` workflow is responsible for building and deploying the Python application to a production environment on every push to the main branch.

The workflow performs the following steps:
1. Checkout the code
2. Set up the Python environment
3. Install the project dependencies
4. Build the Python application
5. Deploy the application to a production server

By automating these CI and CD processes, the project can be developed, tested, and deployed with confidence, reducing the risk of manual errors and enabling faster feedback and iteration.

## Contributing

Contributions are welcome! Please feel free to submit a pull request.
