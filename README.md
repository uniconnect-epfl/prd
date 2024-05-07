## Description

This repository contains an outline template for the PRD.
It also contains a sample PRD under `samples/epfl-pocketcampus` for your reference.

>[!NOTE]
>As you may know, the EPFL Pocketcampus app was developed in the first iteration
>of this course. 

The folder `template` contains the outline for the PRD to get you started.

>[!IMPORTANT]
> When you begin filling out the various sections, you should remove the
> comments added in italics. They are only there to help start your thinking
> process.

## Setup

1. Fork this repo into your organization and clone it 
```
git clone git@github.com:<your-org-name>/prd.git
cd prd
```

2. Setup Github Actions - 

To help you with generating the PDF of your PRD, this repo contains a workflow called `build_pdf.yml`.

To configure the workflow, please change the following lines - 
 
* Team Number

Change the `<Team Number>` to your team's number (e.g., 26) [here](.github/workflows/build_pdf.yml#40).

* Artifact Name 

Change the `<number>` in the PDF name for the Artifact [here](.github/workflows/build_pdf.yml#46).

3. Write your PRD

You can add content to your PRD and push to `main` to generate the PDF. Or you can follow a collaborative workflow of working in branches and making PRs. We trust you can self-organize as a team to achieve this.