# Contributing

Thanks for your interest in contributing to Bloom! This document will guide you through the process of setting up the project locally and making contributions.

## 📖 Table of Contents

+ [📖 Table of Contents](#-table-of-contents)
+ [🌱 Getting Started](#-getting-started)
  + [Prerequisites](#prerequisites)
  + [Setting up the development environment](#setting-up-the-development-environment)
+ [🏃 Running the Project](#-running-the-project)
+ [🔄 Making Changes](#-making-changes)
+ [🚀 Submitting a Pull Request](#-submitting-a-pull-request)

## 🌱 Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Use the [official Flutter docs](https://docs.flutter.dev/get-started/install) to install and set up your Flutter development environment if you haven't already. Currently development is focused on building for macOS.

### Setting up the development environment

1. [Fork the Bloom repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) to copy the entire project to your Github account.

2. Clone the forked repo onto your local machine.

    ```sh
    git clone https://github.com/your_username/bloom_app.git
    cd bloom_app
    ```

3. Set up the original repository on Github as another remote so you can pull changes and manage merging.

    ```sh
    git remote add upstream https://github.com/jessiejalca/bloom_app.git
    ```

4. Before making any changes, install pubspec dependencies from the project's root folder.

    ```sh
    flutter pub get
    ```

## 🏃 Running the Project

To start the development server, simply run:

 ```sh
 flutter run -d macos
 ```

## 🔄 Making Changes

1. Create a new branch for your feature or bug fix. Follow [these naming conventions](https://medium.com/@abhay.pixolo/naming-conventions-for-git-branches-a-cheatsheet-8549feca2534).

    ```sh
    git switch -c new-branch
    ```

2. Make your changes in relevant files.
3. Test your changes thoroughly. Write or adapt tests as needed, and make sure to run them if it applies!
4. Add or change the documentation as needed.
5. Commit your changes with a [good commit message](https://developer.vonage.com/en/blog/how-to-write-a-great-git-commit-message). We use the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/) method to standardize commits for better maintenance, but, in the spirit of KISS, avoid unnecessary capitalization and don't worry about the optional scope that they use.

    ```sh
    git commit -m "<type>: <description>" -m "<optional body>"
    ```

## 🚀 Submitting a Pull Request

1. To ensure a clean pull request, first pull upstream changes into your local repository and merge everything together.

    ```sh
    git switch main
    git pull upstream
    git switch new-branch
    git merge main
    ```

2. Squash your commits into a single commit with Git's [interactive rebase](https://docs.github.com/en/get-started/using-git/about-git-rebase). Create a new branch if necessary.
3. Push your feature branch to your fork on Github.

    ```sh
    git push origin new-branch
    ```

4. Open a pull request from your fork on Github, and wait for your request to be approved. We may ask you to make some changes, but it's only a matter of time before you can consider yourself an open-source contributor!
5. Once the pull request is approved and merged, you can pull the changes from `upstream` to your local repo and delete your extra branch(es), then just keep hacking 😎.
