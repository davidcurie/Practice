# Master Branch

This is a junk repository meant for practicing collaboration between new git users.

If present, the README file of any project will be displayed in your browser by default when you navigate to this repository online.

## Useful resources

- Git-It tutorial: <https://github.com/jlord/git-it-electron>
- GitHub Desktop: <https://desktop.github.com>

### Learning the tools

- GitHub Flow: <https://guides.github.com/introduction/flow/>
- Branching best practices : <https://nvie.com/posts/a-successful-git-branching-model/>
- GitHub Pages: <https://pages.github.com>
- Git Cheat Sheet: <https://www.git-tower.com/learn/cheat-sheets/git/>


-----

## Getting this repository on your local machine

1. Make sure git is installed on your machine.
    - [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. Click the green `Code` button in the top right of this repository.  
3. Select the protocol with which you want to interact with this repository. Clone via https is generally recommended for beginners. Copy this URL to your clipboard.  
4. Open a terminal and navigate your working directory to your desired location for where you want to paste this project.
5. Paste this repository as a directory by entering the following command in your terminal:
    ```bash
    git clone URL
    ```
where URL is the stored URL in your clipboard.

> NOTE: If you don't plan on needing continuous updates of this repository, you can instead extract the ZIP file of this repository onto your machine. Changes you make to contents of this ZIP file will never be reflected in the online repository unless you explicitly take extra steps. This method is ideal if you don't want to install git and just need a copy of someone's code.

After completion of the above steps, you should see the files from this directory on your local machine. Changes you make to these files will not be reflected in the online repository until you explicitly sync changes.

To delete a repository on your machine, simply delete the folder of the extracted files. You will not affect upstream projects, but you will lose the ability to track changes from when you cloned it last.


-----

## Editing files in this repository

EXAMPLE: Add your name to this README file and push it to this repository.
> This example assumes you have cloned this repository as outlined in the steps above. Start this example in the terminal that has its working directory already located to where this repository was extracted.

1. Get the latest version from the servers
    ```bash
    git pull
    ```
2. Edit the file locally on your computer
3. Stage updated file(s) to git
    ```bash
    git add README.md (File2.md File3.ipynb ...)
    ```
    or instead add all modified files at once with
    ```bash
    git add .
    ```
    or
    ```bash
    git add -A
    ```
4. Commit (update snapshot) of your personal repository with your staged changes
    ```bash
    git commit -m "Your update message here"
    ```
5. Tell the servers about your updated changes
    ```bash
    git push
    ```

### Add your name here and see it reflected in this repository

David Curie  
Brian Lerner  
Terry Phang
Alex Toyryla  

-----

## Other Useful Commands

- To check the status of your staging directory before you commit, run the following command:
    ```bash
    git status
    ```
    - This will tell you what branch you are on along with the files git knows you have changed since your last commit or pull. Files you have changed but not staged for commit appear in red. (This means your next sync won't update that file if you push.) Files that are ready to be committed will appear in green. This means tracked changes are up to date and the changes from the next commit will be included in the history of changes for that file.
- To check the explicit changes you made to a staged file since your last commit, run the following command
    ```bash
    git diff --staged SampleFile.ext
    ```
    - This will list the contents of the specified file as it appeared when you added it to your staging directory. Lines that have been added since the last commit will appear in green; lines that have been removed will appear in red. Untouched lines will not be formatted. There are other arguments that allow you to only see new additions/subtractions (suppressing display of unchanged lines) or to show differences word-by-word instead of line-by-line. For example,
    ```bash
    git diff --staged --word-diff <file>
    ```
    will highlight only changed words (useful for essays). See documentation for more arguments.
    - If no file is given as an argument, the contents of all staged files are listed sequentially in the terminal.
    - If you want to look at the difference between your current file, irrespective of whether it has been staged, and the last committed version, you can simply run
    ```bash
    git diff <file>
    ```
- To restore a staged file back to its state during the last commit:
    ```bash
    git restore SampleFile.ext
    ```
    - This will discard changes you made since the last commit, and it cannot be undone.
    - If you instead mean to remove an edited file from the staging directory (and thus prevent the changes from showing up in the next commit cycle) but keep the changes locally intact on your computer, you can run instead:
    ```bash
    git restore --staged SampleFile.ext
    ```
    - See more info here: <https://www.git-tower.com/learn/git/commands/git-restore/>
> Note that you cannot restore back to a previously uncommitted change. You may edit files after they have been staged but before they have been committed. If you want those new edits to be committed, you need to re-add the file to the staging directory. It is also not possible to view a diff log of files that have been added to the staging directory multiple times. If you overwrite your previously staged file in the staging directory with your current edits, you will not be able to see a diff between your newest edits and previous edits. You will still be able to view the newest edits against the last commit.

> Treat commits as periodic checkpoints. You could be extra pedantic and commit after thoughtful change. For example, if tracking a dissertation, you could commit after every paragraph to keep a log of all new ideas. You could instead commit after each re-write; this would keep your history of changes more manageable but you lose the ability to selectively bring back parts of one version into another version.
