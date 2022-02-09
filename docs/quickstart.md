# Quickstart

## Instructions

1) Install git
    - Dowload and run the installer from [git-scm.com](https://git-scm.com)
        - Note (Windows Only): Accept all of the defaults during the installation process
2) Generate an SSH key
    - Sign into [Github](https://github.com)
    - To generate a key, follow the instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
    - To add the newly generated key to Github, follow the instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
3) Create a repository
    - Sign into [Github](https://github.com) (if not already signed in)
    - In the upper-left, click the `New` button next to `Repositories:` or go [here](https://github.com/new)
    - Enter a repository name and hit the checkbox for `Initialize this repository with a README`
    - Hit `Create repository`
4) Clone your new repository to your machine
    - Windows - Open the `git-scm` command line tool that was installed with git in Step 1
    - macOS/Linux - Open your terminal of choice
    - Navigate to the local folder where you will store your git projects
    - Run the following command and replace the Github profile and repository name accordingly:
        - `git clone git@github.com:[profile]/[repository].git`
            - Ex: `git clone git@github.com:nate0000:test.git`
5) Make some changes to the files
    - Navigate to the newly created folder
        - You will see an empty directory with a file called `README.md` (more on that below)
    - Use your favorite text editor or IDE to create some files
6) Sync changes back to the repository
    - In your command line tool of choice, do the following
    - `git add .` - This stages all of the files in this local repository that have been modified/created
    - `git commit -m "Some kind of meaningful commit message` - This actually commits the files with a message saying why they were modified/created
    - `git push -u origin` - This takes the files that have been committed and pushes them to the main branch of the repository.
7) Confirm the changes in Codehub
    - Head back to your repository in Codehub and refresh the page
    - You should now see the newly created files in the repository

### Success!

You have now successfully created a repository, cloned it to your local environment, made some changes, and updated the remote repository with those changes. This is basis for most interactions with git.

## Additional Notes

### Markdown and README.md

From the instructions above, you may remember the `README.md` file that was cloned down with your repository, as well as the note earlier about ensuring that the README file was created with the repository. README files, or some equivalent, are a common artifact found in version control systems. They exist to inform the viewer of the repository's purpose, and can often include other details and guidelines.

Markdown (.md) is a lightweight markup language used to help format text quickly and easily. It is widely used and can usually be found at the front of any git repository, which renders the contents of `README.md` unless otherwise specified. It can also be used for general documentation, like what you are reading now. This is all written in Markdown and rendered by Github.

Here are some examples of Markdown, but it's best to look at the semi-official guide [here](https://markdownguide.org/basic-syntax/) for the basics, and [here](https://www.markdownguide.org/extended-syntax/) for more advanced use cases.

```md
# Heading 1
## Heading 2
...
###### Heading 6

***bold text***

*italic text*

> An example blockquote

1) First item
2) Second item

- First item
- Second item

* First item
* Second item
```