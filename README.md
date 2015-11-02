# Studygroup
## Merging pull requests
When edits are made to the same file in two different branches, it is tricky trying to save changes from both. In an ideal world, you would never allow this scenario to take place, but this is not an ideal world. It is easiest to avoid conflicts if you always create a new branch from the master before you begin, and then push your changes back before anyone else has had a chance to do the same! If you know someone else is working on the same file, or if you need to work on the same file in two different contexts, things can get ugly.

So far the best workflow I've found for conflict resolution is this:

1. Attempt to execute the pull request - it fails, but there are two links. One opens up some command line instuctions, the other launches GitHub on the local machine. Choose the open option.
2. On the local side, synch the branch from the master. You get an error message.
3. Open the offending file(s) using your text editor of choice. You don't get two files which you can compare, but one file with some odd markup separating the edits from the two sources. 
4. Clean up the code. I can see this being genuinely impossible for a big file with lots of edits.
5. Commit the changes back to the branch that contained the commit conflicts.
6. Synch with remote
7. Go back to GitHub and perform the commit.
8. Check to see that you got what you expected.

This does not actually seem like a useful workflow. Far better would be to perform a side-by-side comparison of the two files before executing any pull requests. Better yet would be if files were never edited simultaneously, but that can be hard to achieve.

Anyway, that's what I've learned today.

