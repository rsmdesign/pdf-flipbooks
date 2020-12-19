# PDF Flipbooks

To create or edit a PDF flipbook, follow these steps:

## 1. Setup

### 1.1. Install Git

Follow [this tutorial](https://github.com/git-guides/install-git) to install Git on your computer.

### 1.2. Request access to the GitHub organization

If you already have a GitHub account, [sign in](https://github.com/login). Otherwise, [create a new account](https://github.com/join).

Once you’re logged in, request access to the “rsmdesign” GitHub organization by contacting Will Heinze.

### 1.3. Clone this repository

Next, you’ll need to make a copy of this repository on your computer. To do this, open the Terminal application and navigate to the location on your computer where you want the files to live. One option is to paste the following command:

```
cd ~/Documents
```

On Mac and Linux systems, this puts you in your Documents folder. Once you’ve done this, paste the following command:

```
git clone https://github.com/rsmdesign/pdf-flipbooks.git
```

This will prompt you to enter your GitHub username and password. Note that when you’re typing your password, nothing will show up on the screen – neither the actual text of your password, nor any asterisks or other placeholder characters. This is for your own security. Just type your password when prompted and hit `return`.

## 2. Create or edit a flipbook

### 2.1. Create a flipbook

First, place your new PDF file in the `pdfs` folder. Then, in the repository’s root directory, make a copy of one of the previous flipbooks’ HTML files, such as `dana-point-harbor.html`. It’s imperative that you work from a copy, rather than overwriting the original!

Once you’ve created a copy, rename it. The filename, minus the `.html` file extension, will be used as the URL slug for the new flipbook, so think carefully about this.

Finally, open your HTML file in a text editor such as VS Code or TextEdit. You’ll need to edit two lines in the file:

1.  Go to line 7 and change the page title in the `<title>` tag.
2.  Go to line 16 and change the filepath to match your new PDF.

### 2.2. Edit a flipbook

Editing a flipbook is much the same as creating a new one, except this time you’ll work on the original HTML file instead of a copy.

### 2.3. Publish your changes

There are a few steps to publish your work. First, add all your new files to Git. To check which files need to be added, paste the following command into your terminal:

```
git status
```

This will output a list of files with “unstaged changes”. You’ll need to stage these file by typing the following command into your terminal:

```
git add <filepath1> <filepath2> <...> <filepathN>
```

Replace the filepaths in brackets with the filepaths output from `git status`.

Once you’ve done this, you need to “commit” your changes to the Git repository. To do this, type the following command:

```
git commit -m "Your commit message here"
```

Replace the commit message with a description of what you’ve added or changed.

Finally, “push” your changes to the GitHub repository by entering the following command:

```
git push
```

### 2.4. Check your results

You can verify that you’ve completed this process successfully by navigating to the new or revised page in your web browser. Note that you may have to clear your cache before the changes will take effect. Or, you can navigate to the page in a private browser window.