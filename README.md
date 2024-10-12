# Introduction
This repository contains examples of reusable workflows and composite actions. Reusable workflows and actions help avoid duplication. The repository https://github.com/workflows-and-actions/test-reusable-workflows-and-actions demonstrates how to use these reusable workflows and actions. Github has excellent docs on this subject at https://docs.github.com/en/actions/sharing-automations.

# Main features

## Reusable workflows

- Reusable workflows must reside in the ".github/workflows" directory, subdirectories are not allowed.
- Reusable workflow as a job, not as a step, of the caller workflow and it consists of one or more jobs.

## Composite actions

- Having multple actions in one repo is allowed with the condition that each action resides in its own directory and it is not published for public.
-  For publically available actions, each repo can have only one action.
-  We must have an action.yml file for each action.
-  actions cannot have jobs and must be called as a step of a job.
