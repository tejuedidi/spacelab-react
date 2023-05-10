<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/spacelabdev/spacelab-react">
    <img src="Images/logo.jpeg" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Developer Docs</h3>

  <p align="center">
    <br />
    <a href="https://github.com/spacelabdev/spacelab-react/blob/main/README.md"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="http://spacelab.space/">View Demo</a>
    ·
    <a href="https://github.com/spacelabdev/spacelab-react/issues">Report Bug</a>
    ·
    <a href="https://github.com/spacelabdev/spacelab-react/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">Introduction</a>
      <ul>
        <li><a href="#builtWith">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#gettingStarted">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a>
        <ul>
            <li><a href="#ticketsAndBugs">Tickets and Bugs</a></li>
            <li><a href="#branchesAndPullRequests">Branches and Pull Requests</a></li>
            <li><a href="#styleGuide">Style Guide</a></li>
            <li><a href="#codingConventions">Coding Conventions</a></li>
        </ul>
    </li>
  </ol>
</details>

<!-- INTRODUCTION -->

## Introduction

<a href="https://github.com/spacelabdev/spacelab-react">
    <img src="Images/banner.png">
</a>

Welcome to the developer guide for Spacelab!

This guide is intended to provide instructions on how to contribute to the project, including coding conventions and style guidelines that ensure consistency throughout the codebase. By following these guidelines, you can help us create a high-quality project that is easy to update and maintain.

Whether you are a seasoned developer or just starting out, this guide will provide you with the information you need to contribute effectively to the project. If you are new to Spacelab please read through this document carefully!

Let's get started!

### Our Website is Built With

-   [React.js](https://reactjs.org/)
-   [Sass](https://sass-lang.com/)
-   [Node.js](https://nodejs.org/)
-   [Bootstrap](https://getbootstrap.com)

<!-- GETTING STARTED -->

## Getting Started

To get a local copy of the project, follow these steps.

### Prerequisites

To Run locally, you will need to use any node version >= 14 <= 16. Any other version you may receive an error. If you are using a mac you can install nvm to manage your node versions. (I suggest getting this if on Mac or Linux). For windows, you can use nvm for Windows: https://github.com/coreybutler/nvm-windows

-   nvm
    ```sh
    nvm install 14
    nvm use 14
    ```

### Installation

1. Clone the repo
    ```sh
    git clone https://github.com/spacelabdev/spacelab-react
    ```
2. Install NPM packages
    ```sh
    npm install
    ```
3. Spin up the Project

```
npm start
```

## Contributing

To get started contributing, simply check out the current list of [issues](https://github.com/spacelabdev/spacelab-react/issues) and claim something to work on!

### Tickets and Bugs

We use Github to track updates that need to be made to the website. If you notice a bug, please create a ticket for it right away, so it doesn't get lost or forgotten.

All tickets should be labelled for clarity. The exsisting labels and their purposes are:

-   New Feature: For a new feature or component
-   Enhancement: Improvement to be made to an existing feature or component
-   Bug: Some styling or functionality is broken on the website
-   Documentation: Improvements or additions to documentation
-   Good First Issue: Easy task, good for newcomers
-   Help Wanted: Stuck on something or need a fresh pair of eyes

### Branches and Pull Requests

To get started fixing a bug or creating a new feature, please checkout a new branch.

**Never push directly to main, always use a feature branch!**

#### Creating a Feature Branch

Naming Conventions:

-   feature/nameOfFeature: New feature or comoponent
-   enhancement/nameOfFeature: Enhancement of exsisting feature or component
-   hotfix/nameOfBug: Quick bug or update

To check out a new branch:

```
git checkout -b feature/amazingFeature
```

#### Rebasing a Feature Branch

Say you and another developer have checked out feature branches and happen to both edit the same file. When you go to submit your pull request, you will likely end up with merge conflicts because Git doesn't know which changes to apply.

To avoid merge conflicts, it's good practice to consistently "rebase" (or update) your branch with the current version of main. To rebase a feature branch, follow these steps:

In main:

-   git pull
-   git fetch --all

Switch to Feature Branch:

-   git checkout nameOfFeatureBranch

In Feature Branch

-   git rebase origin/main (in feature branch)

**At a minimum, you should rebase every time a change or update is pushed to main.**

#### Submitting a Pull Request

In general, the flow for creating a new feature goes like this:

1. Update your local version of main: (`git pull`) (in your main branch)
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request and include a screenshot of the feauture you worked on

**Don't forget to delete your branches once they're merged.**

### Style Guide

Please refer to [globalStyles](https://github.com/spacelabdev/spacelab-react/blob/main/src/globalStyles.scss) as it contains color pallettes for the website as well as default styles for headings, buttons, inputs, etc.

In general, developers should try to follow designs from the UX/UI team as closely as possible (down to the pixel if you can).

If a piece of a design isn't possible, or if the design looks funky when translated into code, please message the UX designer who created it to let them know. Until they can redesign that portion, use your best judgement to fix the issue.

### Coding Conventions and Guidelines

**Some of these conventions haven't been implemented throughout the entire site yet, so if you see a piece of code that doesn't match these guides, please update it:)**

Naming Conventions:

1. As per convention, all React component names and file names should be capitalized.

2. For css classes use hypen deliminated strings, for example: .example-class

3. Otherwise, please use CamelCase for everything including:

-   folder names
-   file names
-   variable names
-   function names

Coding Conventions:

1. Components should be designed mobile first and tested thoroughly. Breakpoints are set at:

-   576px for portrait phones
-   768px for tablets
-   992px for laptops
-   1200px for large devices

2. Please do not use let or var to declare your variables, use const instead.

3. In general, try to keep code modular and reusable!

### Thank You For Reading and Welcome to Spacelab!

<p align="right">(<a href="#top">back to top</a>)</p>