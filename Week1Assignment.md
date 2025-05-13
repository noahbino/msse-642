My own knowledge

Git is a version control software that makes it easy for large teams to work on a project. GitHub allows you to create repositories and push file changes to a branch and merge branches to compile work. Git makes it easy to work on the same file or even line with options to choose which changes to keep via merge conflicts.

ChatGPT response to part 1:

🧠 How Git Works — High-Level Overview

⸻

🔁 Types of Version Control Systems

There are three main types of version control systems (VCS):
	1.	Local VCS:
	•	Simple databases on your computer to track file changes.
	•	Example: RCS (Revision Control System).
	2.	Centralized VCS (CVCS):
	•	A single server stores all versions of the code.
	•	Clients check out and commit changes to the central server.
	•	Example: Subversion (SVN), Perforce.
	3.	Distributed VCS (DVCS) — Git falls into this category:
	•	Each user has a full copy of the repository, including its entire history.
	•	Changes can be made locally and later pushed to a remote repository.
	•	Advantage: Work offline, fast operations, and strong collaboration features.

⸻

📸 Snapshots (not diffs)

Git doesn’t store data as changes or diffs. Instead:
	•	Each commit is a snapshot of the entire project.
	•	If files haven’t changed, Git stores references to the same data (for efficiency).
	•	This model makes Git extremely fast and reliable.

⸻

📦 What is a Repository?

A repository (repo) is a data structure used by Git to store metadata and object database for your project.

There are two main types:
	•	Local repository:
	•	Exists on your local machine.
	•	Includes your working directory, staging area, and .git folder.
	•	Remote repository:
	•	Hosted on a server like GitHub, GitLab, Bitbucket.
	•	Shared with collaborators.

You can sync between local and remote repos using commands like git push and git pull.

⸻

✅ What is a Commit?

A commit is a saved snapshot of your project’s files at a specific moment.
	•	Each commit has a unique SHA-1 hash.
	•	Includes metadata: author, timestamp, commit message.
	•	Commits are linked together to form a commit history.

Think of commits as a timeline of your project.

⸻

📂 What is the Working Directory?

The working directory is the current state of your project files:
	•	It’s the folder where you make changes.
	•	Files here are either:
	•	Tracked: Known to Git and under version control.
	•	Untracked: Not yet added to Git.

⸻

🗂 What is the Staging Area (Index)?

The staging area is like a clipboard or prep zone for your next commit.
	•	You add files to it using git add.
	•	When you git commit, only files in the staging area are included.
	•	This gives you control over what to include in each commit.