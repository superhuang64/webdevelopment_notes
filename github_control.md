github 
fully delete a local git repository  `rm -fr .git`
or unhidden .git and remove it

add multiple projects to one GitHub repository
two common approaches
(based on the relationship between the projects)
1. **Subdirectories**:organize each project within a separate subdirectory in the repository. 
steps:
   a. Create a new repository on GitHub.
   b. Clone the repository to local machine:
      ```
      git clone <repository_url>
      ```
   c. Create a new subdirectory for each project within the cloned repository:
      ```
      mkdir project1
      mkdir project2
      ```
   d. Move the files and directories of each project into their respective subdirectories.
   e. Terminal: navigate to the repository's root directory and add, commit, and push the changes to GitHub:
      ```
      cd <repository_directory>
      git add .
      git commit -m "Added project1 and project2"
      git push
      ```

2. **Branches**: Another approach is to use separate branches for each project. This can be useful when the projects are not related to each other. Follow these steps:

   a. Create a new repository on GitHub if you haven't already done so.

   b. Clone the repository to your local machine using the following command:
      ```
      git clone <repository_url>
      ```

   c. Create a new branch for each project:
      ```
      git branch project1
      git branch project2
      ```

   d. Switch to each branch and add the files specific to that project:
      ```
      git checkout project1
      # Add project1 files
      git add .
      git commit -m "Added project1"
      git push --set-upstream origin project1

      git checkout project2
      # Add project2 files
      git add .
      git commit -m "Added project2"
      git push --set-upstream origin project2
      ```

   Each project will have its own branch within the GitHub repository, allowing you to switch between branches to work on different projects.

Choose the approach that best suits your needs based on the relationship between the projects.

tutorial
add a submodule to github repository as reference
:have two GitHub repositories and you want to make one a git submodule of the other
[youtube](https://www.youtube.com/watch?v=eJrh5IjWSGM)