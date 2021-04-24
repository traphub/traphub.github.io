# Branches
* `master`:
The master branch shall include finalized and review information only.
* `branches`:
Contributors shall prepare the new content in respective branches.

# Merge requests
The master branch is protected, such that directly pushing commits to `master` is disabled and merging is allowed for maintainers only. Create a new branch for a new feature and open a merge request which has to be assigned to one of the repository maintainers when the branch is ready to be merged. After review and approval, the new branch is merged into `master` by a squash merge and the development branch is being deleted.

Merging is blocked as long as the merge request's title starts with `WIP` or `[WIP]`, which indicates "work in progress". Remove this prefix to  unblock merging, when the merge request is ready.

# Templates and instructions per section

## Ion Traps

* For each new contribution, please create a new folder within the `ion traps` folder with a suitable name.
* Within this folder, create a suitable markdown file based on the [template for ion traps](ion_traps/template_ion_trap_description.md).
* Once completed, please ensure that the documentation is linked below.

## Passive electronics

* For each new contribution, please create a new folder within the `passive electronics` folder with a suitable name.
* Within this folder, create a suitable markdown file based on the [template for passive electronics](passive_electronics/template_passive_electronics_description.md).
* Once completed, please ensure that the documentation is linked below.
