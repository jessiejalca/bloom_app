# Contributing

Thanks for your interest in contributing to Bloom! This document will guide you through the process of setting up the project locally and making contributions.

## Table of Contents

- [Contributing](#contributing)
  - [Table of Contents](#table-of-contents)
  - [🌱 Getting Started](#-getting-started)
    - [Prerequisites](#prerequisites)
    - [Setting up the development environment](#setting-up-the-development-environment)
  - [🏃 Running the Project](#-running-the-project)

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

<!-- ## 🔄 Making Changes

1. Create a new branch for your feature or bug fix.
2. Make your changes in relevant files.
3. Test your changes thoroughly.
4. Commit your changes with a descriptive commit message.

## 🚀 Submitting a Pull Request

1. Push your changes to your forked repository. -->