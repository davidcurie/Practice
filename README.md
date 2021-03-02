# Master Branch

This is a junk repository meant for practicing collaboration between new git users.

## Getting this repository on your local machine

1. Make sure git is installed on your machine.
    - [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. Click the green `Code` button in the top right of this repository.
3. Select the protocol with which you want to interact with this repository. Clone via https is generally recommended for beginners. Copy this URL to your clipboard.
4. Open a terminal and navigate your working directory to your desired location for where you want to paste this project.
5. Paste this repository as a directory by entering the following command in your terminal:
```
git clone URL
```
where URL is the stored URL in your clipboard.

> NOTE: If you don't plan on needing continuous updates of this repository, you can instead extract the ZIP file of this repository onto your machine. Changes you make to contents of this ZIP file will never be reflected in the online repository unless you explicitly take extra steps. This method is ideal if you don't want to install git and just need a copy of someone's code.

After completion of the above steps, you should see the files from this directory on your local machine. Changes you make to these files will not be reflected in the online repository until you explicitly sync changes.

To delete a repository on your machine, simply delete the folder of the extracted files. You will not affect upstream projects, but you will lose the ability to track changes from when you cloned it last.

## Editing files in this repository

EXAMPLE: Add your name to this README file and push it to this repository

1. get the latest version from the servers
    ```
    git pull
    ```
2. Edit the file locally on your computer
3. Stage updated file(s) to git
    ```
    git add README.md (File2.md File3.ipynb ...)
    ```
    or instead add all modified files at once with
    ```
    git add .
    ```
    or
    ```
    git add -A
    ```
4. Commit (update snapshot) of your personal repository with your staged changes
    ```
    git commit -m "Your update message here"
    ```
5. Tell the servers about your updated changes
    ```
    git push
    ```

### Add your name here and see it reflected in this repository

David Curie
Brian Lerner  
Terry Phang  

