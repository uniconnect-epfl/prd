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

## Using Github Actions

To help you with generating the PDF of your PRD, this repo contains a workflow called `build_pdf.yml`.

To configure the workflow, please change the following lines - 

1. Team Number

Change the `<Team Number>` to your team's number (e.g., 26) [here](.github/workflows/build_pdf.yml#40).

2. Artifact Name 

Change the `<number>` in the PDF name for the Artifact [here](.github/workflows/build_pdf.yml#46).