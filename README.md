# Sample starter code for AHK evaluation

This repository contains the starter code for the students. In contains all the necessary files and file structure for the student to submit the solution:

- an empty `neptun.txt` for the identification of the student;
- a placeholder `screenshot.png` for the screenshot the exercise requests;
- and the skeleton of the exercise, in the current example, an ASP.NET Core Web Api application.

The code also includes a [GitHub Action definition](https://github.com/akosdudas/ahk-sample-startercode/blob/master/.github/workflows/evaluate.yml) describing the evaluation process. This definition will also be cloned for the students when their repository is created. The students are required to create a pull request into their own repository to trigger the evaluation. This evaluation workflow executes preparation steps (setting up the build environment) and then the [evaluator application](https://github.com/akosdudas/ahk-sample-evaluator) in the form of a Docker image. Finally a [custom action](https://github.com/akosdudas/ahk-action-publish-result-pr) publishes the result into the [pull request thread](https://github.com/akosdudas/ahk-sample-studentsolution/pull/1).

The repository also contains a [pull request template](https://github.com/akosdudas/ahk-sample-startercode/blob/master/.github/pull_request_template.md). The text content of this file will be used by GitHub to populate the description of the _pull request_ when the student creates it. It serves as a reminder of what to do.
