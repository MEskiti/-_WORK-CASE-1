
#  Заголовок 1-го рівня
























































##What is a Commit? A commit is the fundamental unit of data storage in Git. It represents a logically complete snapshot of all project files at a specific point in time.
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
