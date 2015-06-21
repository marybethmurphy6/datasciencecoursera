## This is a markdown file

Here is some regular text.
* here is a bullet
* here is another bullet

[Here is a sample of a link](https://www.coursera.org/)

###Excellent Tips for Using Git/GitHub:



This is video #8 in the Data School series, "Introduction to Git and GitHub." Relevant links, a command list, and the full transcript are below (published May 3, 2014). Playlist: http://www.youtube.com/playlist?list=PL5-da3qGB5IBLMp7LtN8Nc3Efd4hJq0kD 

#####== LET'S CONNECT! ==

* [Blog: http://www.dataschool.io] (Blog: http://www.dataschool.io)
* [Newsletter: http://www.dataschool.io/subscribe/] (Newsletter: http://www.dataschool.io/subscribe/)
* [Twitter: https://twitter.com/justmarkham] (Twitter: https://twitter.com/justmarkham)
* [GitHub: https://github.com/justmarkham] GitHub: https://github.com/justmarkham

#####== LINKS RELATED TO THIS VIDEO ==

* Git quick reference for beginners: http://www.dataschool.io/git-quick-reference-for-beginners/
* Tracking, staging, and committing: http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository
* Markdown Live Editor: http://jrmoran.com/playground/markdown-live-editor/
* Mastering Markdown: https://guides.github.com/features/mastering-markdown/

#####== COMMAND LIST ==

* create a file: touch [filename]
* check the status: git status
* track and stage a single file: git add [filename]
* track and stage all files: git add .
* commit with a message: git commit -m "description of commit"
* view the log: git log
* push changes: git push [remotename] [branchname]

#####== TRANSCRIPT ==

In this video, we're going to continue working with the "test-repo" we created previously. Specifically, we're going to edit an existing file, add a new file, commit those changes, and push those changes up to GitHub.

To start, we've already opened up Git Bash and changed our working directory to test-repo. As you might recall, there's just one file in the repo, which is the "README.md" file. We're going to edit that file.

Since it's a Markdown file, you can edit it in any text editor. I've opened the file in Windows Notepad, and am just going to make a simple edit and then save the file.

Let's also create a new Markdown file called "new.md". We're going to use a command called "touch". It's not a Git command, but it's especially handy on Windows since it can be hard to create a file with a non-standard extension. Simply type "touch" and then the name of the file. You can see that it has been created.

The file we created is empty, so let's open it in Notepad.

I've written some Markdown code in this Markdown Live Editor, so that you can see a preview of what it looks like. The Markdown code is on the left, and the rendered version is on the right. I'll link to this tool in the video description.

Anyway, let's copy the Markdown code to the new.md file and save it.

We're back in Git Bash, and are going to run the "git status" command to see the status of our files. It tells us that we've got one tracked file that has been modified, and one untracked file that has been added.

We want to stage both of these files for committing. We use the "git add" command to do this. You could do this one file at a time using "git add" and then the filename. But instead, we're going to use "git add ." which adds both of them at once.

Let's run the status again. We can see that the changes are ready for committing.

To commit, use the "git commit" command. We use the "-m" argument and write a message because every commit should have a descriptive message.

The commit is complete, and we can run "git status" to confirm that there is nothing else to commit. We can also check the log to see that the commit is there.

Everything we've done so far has only affected our local machine. To get our GitHub repo up-to-date, we need to push up our changes.

To push our changes, we use the "git push" command. The specific command is "git push origin master", which means that we want to push the "master" branch to the "origin" remote. Remember that in a previous video, we set up the "origin" remote to refer to our GitHub repository.

Type in your password, and you're done. Refresh GitHub, and you can see that the "README.md" file has been modified, and the "new.md" file has been added. You can also see the commit history.

On my blog, dataschool.io, I've got a Git quick reference guide that I wrote specifically for beginners, containing these and other common commands. I'll link to it in the video description, and hopefully you'll find it to be useful.