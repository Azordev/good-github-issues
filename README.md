#### _Read this in other languages_

<kbd>[<img title="Española" alt="Española" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/es.svg" width="22">](README.es.md)</kbd>

- [Issues](#issues)
  - [What is an issue?](#what-is-an-issue)
  - [What should an issue contain?](#what-should-an-issue-contain)
    - [Description](#description)
    - [Screenshots:](#screenshots)
    - [Checklist:](#checklist)
    - [References:](#references)
  - [What should you consider when writing an issue?](#what-should-you-consider-when-writing-an-issue)
    - [One issue per issue](#one-issue-per-issue)
    - [Titles are important](#titles-are-important)
    - [If applicable, do not forget to add](#if-applicable-do-not-forget-to-add)
- [Bibliografía:](#bibliografía)

# Issues

[Azordev](https://github.com/Azordev/) manages almost all of its work through GitHub. So it’s important that we write well-crafted, detailed issues. Here are some best practices for writing proper GitHub issues.

Good issues will get you more help by making it easy for outside contributors to understand your project and help you out.

## What is an issue?

When we talk about issues, we're talking about problems, this problems can arise in various ways, including discussions about what technology to use in a project or how to organize its file structure.

An issue represents one task or problem that needs solution to move the project forward, and can be addressed to a developer, designer, copywriter, or anyone inside or outside the project with the ability to solve it.

Tasks must always be well explained so that someone who doesn't belong to the project can take them and collaborate without problems.

For this you can follow the following guide, which will be divided in two parts, one talking about the content that an issue must have, and another that talks about things to consider to create a good issue.

## What should an issue contain?

### Description 

The first thing you should add to your issue is a clear description of the problem, preferably seen from a user's point of view, known as [User story](https://en.wikipedia.org/wiki/User_story).

We usually stick to the following structure for the issue's description:

- Context: explain the conditions which led you to write this issue. — “Since we’ve moved to the latest version of Express.js, we’ve experienced a few performance issues (#14 and #15) on production.”
- Problem or idea: the context should lead to something, an idea or a problem that you’re facing. — “We’ve had no way of easily seeing the performance impact before releasing our changes to production.”
- Solution or next step: if you have an idea of how to proceed with the problem, you can add a solution, if not, you can add a next step. — “Please help us to find which tools are good to measure the performance of a server in NodeJs”

### Screenshots:

Whenever applicable, you should add screenshots about what you're referring to in the issue, to give the developers more context and everyone can better understand the problem being discussed.

### Checklist:

Possibly the most important part, since it is where are the points that the developer looks when solving the problem.

You can think of the checklist as the list of minimum parameters that must be met for a problem to be considered solved.

### References:

Since issues should be kept short, references will be a foothold where developers can go for more information than what is provided in the issue. 

If it's a complex issue, you can add documentation or anything that can help the developer to take the next step. 

An example of use is when we ask to add styles to a web page and we rely on a design, either in figma or adobe xd or if it is in a PDF, we can add the link to this design, apart from the screenshots in their respective section. 

## What should you consider when writing an issue?

### One issue per issue

It’s also important to avoid issues that describe too much. Each bug or feature request should be documented in its own issue.

- Bad — “The form needs a subject field. Also, the submit button is broken.” (Separate these into two issues.)
- Good — “Add a subject field to form”
- Good — “Submit button causes 405 error”

It’s often unavoidable that issues are complex, especially with big feature requests. Adding a lot of detail to an issue is great! But when a complex issue can be separated into multiple issues, that makes them easier to resolve.

### Titles are important

Keep your titles short and descriptive. Don’t try to cram every bit of information in the title.

For example, instead of writing the title “Search input causes error when you type over 50 characters and press enter”, use something shorter like “Search errors on 50-character submit.” The specific details — like the error happening when you press enter — can be explained in the issue comment.

### If applicable, do not forget to add 

- **Links** — Include links to the specific application views you’re describing.
- **Screenshots** — A picture is worth 1,000 words (a GIF is worth 1,000,000). A screenshot can help clarify the issue you’re seeing.
- **@ me** — If you know there are certain people that should be alerted, be sure to mention them in the issue.
- **Labels** — Use the labels to classify your issues, too u can use it to create some easy way to filter it. I suggest three types of labels: 

  1. **Effort estimation:** Talk about how much effort require the label to be completed. You can follow [this guide](https://docs.google.com/document/d/1ZaiuNGsNSQvZgB6Gr20imG9VFEB5YPNDfD5PaDoYPPg/edit?usp=sharing) to check how we handle the effor estimation 
  2. **Type of task:** As mentioned in [What is an issue](#what-is-an-issue), there can be different types of tasks: Tasks for designers, for example, can be labeled `design`, while tasks for developers can be divided by technologies, for example `javascript`, `css`, or they can be divided by type of task, for example: `api`, `logic`, `style`.
  3. **Priority:** This label stipulates how soon an issue is required to be resolved, it can be three or more: `low`, `mid`, `high`

# Bibliografía:

- [Writing a proper issue](https://medium.com/nyc-planning-digital/writing-a-proper-github-issue-97427d62a20f)
- [How we write our github issues](https://wiredcraft.com/blog/how-we-write-our-github-issues/)
- [Effort Estimation guide](https://docs.google.com/document/d/1ZaiuNGsNSQvZgB6Gr20imG9VFEB5YPNDfD5PaDoYPPg/edit?usp=sharing)