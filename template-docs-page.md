# Documentation template instructions

An example template that you can use to provide best-practices for starting a new how-to document.

[**Copy a version of this template without the instructions**](#copy-the-template)

## Frontmatter

[Hugo](https://gohugo.io/) uses a set of metadata at the beginning of each page
called [frontmatter](https://gohugo.io/content-management/front-matter/)
to define website build required info as well as other blog page details.

Frontmatter is strict YAML syntax and must be added to the top of every
page. Example formatting template:

```yaml
---
# This section is called the "frontmatter" for your page
title: "Title for your page" # Use sentence case for titles
linkTitle: "Template: New docs page"
# The linkTitle field (above) is optional; use it to provide a shorter link if your page title is very long
weight: 50 # This affects the placement of the link in the sidebar on the left. Pages are ordered from top to bottom by weight, lowest to highest.
type: "docs" # You won't need to update this.
#aliases:
#  - /docs/example/redirect/moved-renamed-page
#  - /docs/another-example
# Has the page ever moved? If yes, include the prior location above, starting with path from the site root (for example /docs/, /blog/, or /community/). The old URL will redirect to this new file. For a new pages, "aliases" are not required.
---
```

Learn how to do something very cool.

```
<!--
Make sure to state the goal of this **task-oriented
content** and the value proposition for the user (why is this important?).
Example:
Learn how to use X to reduce/improve/etc. your Y and Z.

Generally, make sure you answer the questions:
- "what does this guide show you how to do?"
- "why would someone want to do this?"
-->
```

## Before you begin
```
<!--
State all the requirements in this this section of the document.
Define any assumptions made (avoid tripping up the user and distracting them from the Knative feature you are trying to explain).
This is where you get past any of the non-Knative items so that you can focus on Knative-specific stuff below. For example:
-->
```
To complete the steps in this task, you must ..... meet/have/install/create/? the following:

- A Kubernetes cluster with [Knative installed](./docs/install/README.md).
  <!-- Make sue to use relative links. -->
- The latest version of ... running?
- Privileges to .....
- Any other requirement?

## Break steps into logical sections
```
<!--
Avoid nesting headings directly on top of each other without text/explanation/context between.
-->
```

Introductory statement to define the goal of these steps and the role they play in this document (why its important?):

1. Use ordered lists for steps.

    * Use bulleted lists for options:

       1. Sub step one
       1. Sub step two

    * Option two:

       Explain the value of why a user would choose this option.

1. Step number two.

1. Step number three.

### Use a sub-section to group related sub-tasks
```
<!--
Avoid nesting headings directly on top of each other without text/explanation/context between.
-->
```

Introductory statement to define the goal of this sub-task and why its important:

```
<!--
Put code into code blocks.
Markdown formatting: Use spaces, not tabs to indent code blocks, and leave one blank line before and after the block.
Examples:-->
<!--
1. Here's a code snippet:

   ```bash
   kubectl apply --filename test.yaml
   ```-->
<!--
1. Another inline code snippet with the `kubectl apply` command.
-->
```

## Cleaning up
```
<!--
If this "how-to" guide installs a sample application, creates and runs resources that might cost unnecessary fees, you should show the user how to delete or remove.
-->
```

Run the following command to stop/remove/avoid running this example and prevent incurring fees from your cloud provider/your cluster/etc.

## What's next
```
<!--
Link to relevant topics, if applicable. Once someone has
completed these steps, what might they want to do next?
Remember to keep it focused and targeted, too many links are not as useful.
-->
```

Now that you have an example running, learn how to enable .....:

- [Link](./serving/example.md) <!-- Always use relative links if linking to a page within the Docs repo. -->
- [Link](./eventing/example.md)
- [Link](./search-example.md)


# Copy the template
```yaml
---
# This section is called the "frontmatter" for your page
title: "Title for your page" # Use sentence case for titles
linkTitle: "Template: New docs page"
# The linkTitle field (above) is optional; use it to provide a shorter link if your page title is very long
weight: 50 # This affects the placement of the link in the sidebar on the left. Pages are ordered from top to bottom by weight, lowest to highest.
type: "docs" # You won't need to update this.
#aliases:
#  - /docs/example/redirect/moved-renamed-page
#  - /docs/another-example
# Has the page ever moved? If yes, include the prior location above, starting with path from the site root (for example /docs/, /blog/, or /community/). The old URL will redirect to this new file. For a new pages, "aliases" are not required.
---

Learn how to do something very cool.

<!--
Make sure to state the goal of this **task-oriented
content** and the value proposition for the user (why is this important?).
Example:
Learn how to use X to reduce/improve/etc. your Y and Z.

Generally, make sure you answer the questions:
- "what does this guide show you how to do?"
- "why would someone want to do this?"
-->


## Before you begin
<!--
State all the requirements in this this section of the document.
Define any assumptions made (avoid tripping up the user and distracting them from the Knative feature you are trying to explain).
This is where you get past any of the non-Knative items so that you can focus on Knative-specific stuff below. For example:
-->

To complete the steps in this task, you must ..... meet/have/install/create/? the following:

- A Kubernetes cluster with [Knative installed](./docs/install/README.md).
  <!-- Make sue to use relative links. -->
- The latest version of ... running?
- Privileges to .....
- Any other requirement?

## Break steps into logical sections
<!--
Avoid nesting headings directly on top of each other without text/explanation/context between.
-->

Introductory statement to define the goal of these steps and the role they play in this document (why its important?):

1. Use ordered lists for steps.

    * Use bulleted lists for options:

       1. Sub step one
       1. Sub step two

    * Option two:

       Explain the value of why a user would choose this option.

1. Step number two.

1. Step number three.

### Use a sub-section to group related sub-tasks
<!--
Avoid nesting headings directly on top of each other without text/explanation/context between.
-->

Introductory statement to define the goal of this sub-task and why its important:

<!--
Put code into code blocks.
Markdown formatting: Use spaces, not tabs to indent code blocks, and leave one blank line before and after the block.
Examples:-->
<!--
1. Here's a code snippet:

   ```bash
   kubectl apply --filename test.yaml
   ```-->
<!--
1. Another inline code snippet with the `kubectl apply` command.
-->

## Cleaning up
<!--
If this "how-to" guide installs a sample application, creates and runs resources that might cost unnecessary fees, you should show the user how to delete or remove.
-->

Run the following command to stop/remove/avoid running this example and prevent incurring fees from your cloud provider/your cluster/etc.

## What's next
<!--
Link to relevant topics, if applicable. Once someone has
completed these steps, what might they want to do next?
Remember to keep it focused and targeted, too many links are not as useful.
-->

Now that you have an example running, learn how to enable .....:

- [Link](./serving/example.md) <!-- Always use relative links if linking to a page within the Docs repo. -->
- [Link](./eventing/example.md)
- [Link](./search-example.md)

```
