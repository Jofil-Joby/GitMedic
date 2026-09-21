## Decision and Reasoning

GitMedic decides whether the repository contains a recognizable .gitignore file. When the file is absent, it reports a repository-hygiene finding and recommends adding appropriate ignore rules.

## Inputs and Data Sources

It uses the repository file list and checks for a .gitignore artifact. The decision does not infer what files should be ignored from project semantics.

## Limits and Constraints

It does not prove that an existing .gitignore is complete or correct. Global Git excludes, organization policies, and nonstandard ignore mechanisms are outside the current evidence boundary.
