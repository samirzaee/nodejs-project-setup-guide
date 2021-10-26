# Node.js Project Setup Guide

📄 A step-by-step guide to creating and setting up a Node.js project.

## Step One: Starting the directory(repository)

There are two ways to start the directory:

1.  **Starting the repository on an online Git service (like Github,...):**\
    In this way, (for example on GitHub) we will have these at once:
    -   An initialized git repo with a name
    -   A `README.md` with the repo's short description
    -   The initial commit with above changes
    -   (optional) A `LICENSE` file (Note that the license file could have 
        no file extension or on of `.txt`, `md`, `rst`. The `.md` and the no extesion are the most common options.) (For licenses also [this repo](https://gist.github.com/Rypac/7349957f95f0713143fda2f3d3bc10c8) could be useful.)
    -   A *.gitignore* file (On GitHub for example, you'll get a big 
        *.gitignore* file)

    **Note:** The `.gitignore` you're given by the platform (.e.g GitHub) is a very big one that contains ignores for any cases. You don't need all of them. So need to either delete anything that you don't need or create your `.gitignore` file manually and fill it out through out the the proccess of building the project as you will need it. The basic `.gitignore` file is like this:

    #### **`.gitignore`**
    ```
    /node_modules/
    ```
    Don't forget to commit changes.

    And finally clone the repo (if you didn't yet) and run `npm init` command, go through steps and then 
    commit the changes.

2.  **Starting the directory locally**:\
    Steps needed in this way are:
    
    1.  Create the directory with a proper name
    1.  Run `git init` command to initialize the repo
    1.  Commit changes as the *initial commit*
    1.  Add the `README.md` with a very short description (then commit it)
    1.  Add the basic `.gitignore` file like below:

        **`.gitignore`**
        ```
        /node_modules/
        ```
        and commit changes.

    1.  Initialize npm with `npm init` command, go through steps and then 
        commit the changes. 
        **Note:** The differece here with the other way is that you need to manually add the remote repository address to the `package.json` later. (for example, after your first push)

        You need to add these to your `package.json` file:

        ```json
        "repository": {
        "type": "git",
        "url": "git+https://github.com/samirzaee/nodejs-project-setup-guide.git"
        },
        "bugs": {
        "url": "https://github.com/samirzaee/nodejs-project-setup-guide/issues"
        },
        "homepage": "https://github.com/samirzaee/nodejs-project-setup-guide#readme"
        ```

        Change urls based on yourown remote repo.

    1.  As you probably saw and did in the steps of initializing npm, 
        you have the license field of your `package.json` filled with what you specified. But you don't have a license file in your directory. You can add it using the steps [explained in for Github remote repositories](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository). If your remote repository is not on github you can just use the github steps to get the license text and then copy and paste it to your manually created license file. The license file is like one of these:
        -   LICENSE (prefered - more common)
        -   LICENSE.md (prefered - more common)
        -   LICENSE.txt
        -   LICENSE.rst

        and must be in the root of the directory(/repository). The first two are mostly commonly used options.\
        For licenses also [this repo](https://gist.github.com/Rypac/7349957f95f0713143fda2f3d3bc10c8) could be useful.




