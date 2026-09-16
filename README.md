
Task 1: Purpose of Git, Core Concepts, and Basic Commands

|This part is made by Oleksiy Orlov

Purpose of Git
Git is a Distributed Version Control System (DVCS) created by Linus Torvalds in 2005 to manage Linux kernel development. Its main purpose is to ensure high speed, data integrity, and support for non-linear development workflows involving thousands of parallel branches.

Core Actions and Commands:

'git init' — Creates a new empty local repository in the current directory (creates a hidden .git folder).

'git clone <URL>' — Downloads a copy of an existing remote repository from a server (GitHub, GitLab, etc.) to a local machine.

'git status' — Displays the current state of the working directory (untracked, modified, or staged files).

'git add <file>' — Adds a specific file to the Staging Area (Index).

'git commit' -m "Change description" — Creates a new commit from staged changes with a short description.

'git log' — Lists all commits in the current branch with their hashes, authors, dates, and messages.

'git push <remote> <branch>' — Uploads local commits to a remote repository.

'git fetch' — Downloads new data from a remote repository without merging it into local code.

'git pull' — Downloads new changes from a remote repository and automatically merges them into the current branch(git fetch + git merge).

'git branch <branch-name>' — Creates a new branch.

'git checkout <branch-name>' — Switches the working environment to the specified branch.

'git merge <branch-name>' — Merges the specified branch into the current one.











































##What is a Commit? A commit is the fundamental unit of data storage in Git.
It represents a logically complete snapshot of all project files at a specific point in time.

Unlike centralized version control systems, Git does not store commits as a list of file deltas or patches.
Instead, Git takes a snapshot of what all files in the project look like at that moment and stores a reference to that snapshot.
If a file hasn't changed, Git links to the previously stored copy rather than duplicating it

How a Commit Tracks File Changes
Tracking changes occurs through the interaction of three file states and structural difference analysis:
The Three Git Areas (Three-State Architecture):
Working Directory: Files on disk currently being edited.
Staging Area / Index: An intermediate file in .git that determines which changes enter the next commit.
Git Repository / Object Database: Permanent storage where commits exist as compressed objects.

Diffing Mechanism:
When a file is staged (git add), Git generates a unique content hash.
During commit creation, Git compares the new commit's tree object hash with the parent commit's tree object hash.
If a file hash differs, Git performs a line-by-line comparison and calculates the exact diff (added + or removed - lines).
Data Integrity (Immutability): Due to cryptographic hashing, commit history is immutable. Altering an old commit changes its hash and invalidates subsequent linked commits, ensuring complete reliability when auditing code changes.






















Командна робота Васіна Костяина і Орлова Олексія 
