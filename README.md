# Sample starter code for AHK evaluation

This repository contains the starter code for the students. In contains all the necessary files and file structure for the student to submit the solution. All files are now empty.

The code also includes two GitHub Actions definitions. These will also be cloned for the students when their repository is created based on this repository.

- Workflow [test](https://github.com/akosdudas/ahk-sample-startercode/blob/master/.github/workflows/test-commit.yml) executes a simple verification on every commit if the student has filled in the required `neptun.txt`. For this purpose, a [custom-made GitHub Action](https://github.com/akosdudas/ahk-action-neptuncheck) is referenced. This workflow is also the place to execute basic checks on the student solution, such as verifying if it compiles.

- Workflow [evaluate](https://github.com/akosdudas/ahk-sample-startercode/blob/master/.github/workflows/evaluate-pr.yml) executes the evaluation. This is triggered for pull requests only, so that the evaluation result can be written into the comment thread of the pull request. The students are required to create a pull request into their own repository to trigger the evaluation. This workflow executes the [evaluator code](https://github.com/akosdudas/ahk-sample-evaluator) in the form of a Docker image, then a [custom action](https://github.com/akosdudas/ahk-action-publish-result-pr) publishes the result into the [pull request thread](https://github.com/akosdudas/ahk-sample-studentsolution/pull/1).
