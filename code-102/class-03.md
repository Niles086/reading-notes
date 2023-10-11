# Revisions and the Cloud

## Version Control

Version control is a system that captures snapshots of files, similar to cloud-based office applications. It enables you to revisit earlier versions of a file, even if the original has been overwritten. This allows you to access prior versions and track any modifications, which is particularly valuable for diagnosing and resolving issues.

## cloning in Git

Cloning allows the duplication of all versions of every file within your project. It also grants the ability to clone code from accessible repositories on GitHub, providing access to others' work. This can be especially useful when collaborating on a project or when you require shared resources. Example of the clone command.

                git clone https://github.com/test mydirectory

## Tracking Staged Files

You can track and stage files by using the following commands in the terminal.

               git add filename    or    git add *

## Snapshots of Changed Files

You can take a snapshot of your changed files by using the following terminal commands.

               git commit -m “made change comment added here”

## Uploading Changed Files

You can send your changed files to Github usint the following terminal commands.This command pushes changes from the local master branch to the remote repository named origin.

              git push origin master
