# Contributor's Guide

## Summary

- [Contributor's Guide](#contributors-guide)
  - [Summary](#summary)
  - [Contribution Prerequisites](#contribution-prerequisites)
  - [Getting Started](#getting-started)
    - [Creating a New Component ](#creating-a-new-component-)
    - [Modifying an Existing Component ](#modifying-an-existing-component-)
    - [Emulating an existing component for testing](#emulating-an-existing-component-for-testing)
  - [Submitting a Pull Request](#submitting-a-pull-request)


You can contribute in many ways:
 - Opening or participating on an issue;
 - Reporting a bug;
 - Creating a [pull request](#submitting-a-pull-request).

## Contribution Prerequisites
- Node;
- Docker for the visual tests;
- [`Commitizen`](http://commitizen.github.io/cz-cli/) for commits;

We have .nvmrc, therefore just use [nvm](https://github.com/nvm-sh/nvm) to set the repo default version of Node
```sh
nvm use
```



## Getting Started
<a name="newComponent"></a>
### Creating a New Component <br><br>

1.  #### Fork the project ( [Help Guide to Fork a repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo) );<br><br>
   Clone the project;<br><br>
2. Create a branch specific to the issue you are working on:


    ```sh
    git checkout -b update-readme-file
    ```
3.  Open the project in your prefered text editor, select the file you want to contribute and make your changes;

    When creating a new component, you can use our script to generate initial structure for the new component:

        ```sh
        yarn generate ComponentName
        ```
<br><br>
   

4.  #### Run Unit Tests<Br>
   <p>`--to be included--`</p><br>
5. Run Regression Tests<Br>

   <p>`--to be included--`</p><br>
6. Update Storybook <br>
      <p>`--to be included--`</p><br>
7.  After making your changes in the new git branch, add your modified files to git ( [How to add, commit, push and go(http://readwrite.com/2013/10/02/github-for-beginners-part-2/) ):

    ```sh
    git add path/to/filename.ext
    ```

    You can also include all unstaged files using:
    ```sh
    git add .
    ```

    Note: using a `git add .` will automatically add all files. You can run a `git status` to see your changes, but do it before `git add`.<br><br>

8.  Commit your changes using `commitizen`;
   
    ```sh
    yarn commitizen
    ```

9.  You'll be prompted to fill in any required fields. Your commit messages will be formatted according to the standards defined by project.
    
    - Select the type of change that you're committing *(required)*
    - What is the scope of this change (e.g. component or file name)?
    - Write a short, imperative tense description of the change *(required)*
    - Provide a longer description of the change.
    - Are they any breaking changes? (y/N)
    - Does this change affect any open issues? (y/N)

10. Push your commits to your Fork:

    ```sh
    git push -u origin branch-name
    ```
11. Submit a pull request;
12. PR Approvation Proccess;
13. Publication of the package to `npm`.


<br>

### Modifying an Existing Component <br><br>

[Folow steps 1, 2 and 3 from, New Component Section](#fork-the-project-help-guide-to-fork-a-repository)

4. Run the Storybook of the component to see its behavior;
5. Create the changes and live check in Storybook how it is affecting the component;
6. Follow [step 4 and forward](#fork-the-project-help-guide-to-fork-a-repository) from, New Component Section to commit and create your Pull Request

<Br>  <br>

### Emulating an existing component for testing
TBA

## Submitting a Pull Request

Open your pull request (if you don't know how do it, check this [tutorial](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)).


