# Pega Cloud service release notes template

Pega tech doc created this folder to for service teams to source their release notes folder and use the template in it.

## Goal

To help engineering team write release notes that meet Pega Tech doc guidelines
Internal release notes are the primary guide for Pega Cloud operations, SRT, and GCS to understand new functionality in a service release.

## Process overview

Each service release service PRD produces one release note file per release and maintains a release notes folder within their repository.

Tech doc assists engineering deliver consistent quality information by:

- Creating a simple internal release note template created in markdown format that all service teams will adopt in their local repository to communicate latest features and functionality.
- Helping internal service teams and SRT develop a centrally-located directory for all internal service release notes and required internal service-related SOPs.
- Completes review of latest team-written release notes in their service repository during the service release Plan stage.
- Verifies that updated service release notes are complete and available to Pega Cloud operations.

## Process details

### Required steps

1. Engineering team write release notes/bugs by creating a new or updating an existing the tech doc-provided template.

2. Engineering team pushes the new or updated release note file into a release notes folder in their repository.

3. Pega Tech doc pulls in changes to the release notes file to a local repository and reviews/edits the content.

4. Pega Tech doc pushes the changes for review back to the engineering repository.

5. Engineering team finalizes the final and pushes the changes.

### Templates

The release notes template files in `/internal-release-notes` for each release must include:

- A goal description that includes the following sections:
  - Summary of the business value that is driving this change
  - A hyperlink to the Agile Studio goal
  - Reason update is required now?
  - Do these changes require a Pega Cloud infrastructure update? Yes or no

- Epics in the goal that includes the following details:
  - A hyperlink to the Agile Studio epic
  - Change or enhancement detailing the new feature do?
  - Impact on Pega Cloud Operations: does it improve their experience?
  - Does it require a new or an update to an existing SOP?

- Bug fixes/Issues addressed that includes the following details or sections
  - A hyperlink to the Agile Studio bug
  - Description of the issue
  - Resolution: What was fixed?
  - Why it's required in this new service release? why is it required now and can't wait?
