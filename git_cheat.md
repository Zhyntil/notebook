#Commands related to a remote repository:
git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
git push or git push origin main (Both accomplish the same goal in this context)

#Commands related to workflow:
git add .
git commit -m "A message describing what you have done to make this snapshot different"

#Commands related to checking status or log history
git status
git log

##The basic Git syntax is program | action | destination.

For example,

git add . is read as git | add | ., where the period represents everything in the current directory;
git commit -m "message" is read as git | commit -m | "message"; and
git status is read as git | status | (no destination).

#Git Best Practices

Two helpful best practices to consider are atomic commits and leveraging those atomic commits to make your commit messages more useful to future collaborators.

An atomic commit is a commit that includes changes related to only one feature or task of your program. There are two main reasons to do this: first, if something you change turns out to cause some problems, it is easy to revert the specific change without losing other changes; and second, it enables you to write better commit messages.

As for writing better commit messages, this Chris Beams article on How to Write a Git Commit Message provides excellent guidelines for writing neat and concise commit messages.
