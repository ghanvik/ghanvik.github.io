---
layout: post
title:  "Editing the LibreOffice Base Guide"
date:   2022-03-12 12:00:00 -0700
categories: journal-entries
---
In the past couple of months, I have spent some free time contributing to the [LibreOffice](https://documentation.libreoffice.org/en/english-documentation/) open-source community. Per the suggestion of a member of the docs team, I started by reading through a couple of chapters of the work-in-progress Base 7.3 User Guide. Base is a database frontend similar to Microsoft Access. This journal article discusses my process for editing the guide and what I've learned.

# User Testing

As someone who was unfamiliar with LibreOffice software, I was in a good position to look for flaws in the existing documentation as I attempted to learn the software. I chose to work on Base because I have little experience with databases in general.
To start, I attempted to follow the guide step-by-step and seeing if the instructions worked as they said they would. I was mostly able to follow the steps to the end. Some of the times I could not follow the instructions were bugs in the software rather than problems with the documentation itself. For instance, there was a bug that caused Base to crash when building a form. At this point, the only thing left that I could do was submit a bug report.

In some cases, I could not follow the documentation because of how the content was organized. For example, one page contains a list of possible SQL commands and the following pages elaborate on each command. However, two of the explanations for the first and last commands were combined, with no indication in the text that this had been done. I found this layout hard to follow because when I went looking for a specific explanation, I did not find it. To fix this, I separated the explanation into two distinct explanations. In another case, the guide shows an image of a dialog box and an instruction on which option to choose, but no explanation of what those options mean. I decided to add a sentence to this section that referred to another page that contained an explanation of those options.

# Writing for an Audience

Doing these edits made me think of some of the more subtle ways technical writers might have to think about the audience. In my first example, the original organization had some merit. It took up less space because it grouped together two SQL commands that might be used to accomplish the same thing. However, I chose to separate them because the audience should not be expected to already know the two commands can be used the same way. The audience is also unlikely to read the guide beginning-to-end. They are more likely to look for a specific piece of information to use a specific feature of Base, so it makes sense to separate them to make them each easier to find. When I had trouble making decisions on how to edit, one thing that helped was to ask how a user would be likely to use the text.

I also noticed some weaknesses of paragraphs for communicating use cases. One of the examples in the text was a database for a library that covered two cases: a school library and a public library. The database could be used for either case. However, this would only be clear to a reader if they read the entire section. I ended up choosing to keep the paragraph format because I felt that the lengthier explanation that followed the example could not be communicated any other way. However, I edited the paragraph so that the first thing it said was that the database covered two cases.
