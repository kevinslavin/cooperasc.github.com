The website of [Cooper Union](http://cooper.edu)'s Art Student Council. Powered by [Jekyll](http://jekyllrb.com) and hosted by [Github Pages](http://pages.github.com).

---

## What is Git?

## Why Git?

### Clone / Fork / Push / Pull

Anyone who is a [member of student council](https://github.com/CooperASC?tab=members) can directly create and edit any page on this site by cloning the repository and pushing changes back to Github.

## Contributing to the Cooper ASC Website

### Desktop Git Clients

For those who are not comfortable with Git's command line interface, Github has decent clients for [Mac](http://mac.github.com) and [Windows](http://windows.github.com) that make cloning, pushing, and pulling a single-button affair.

### Editing content online

If you're just looking to create or edit content, you can [edit the site online with Prose.io](http://prose.io/#CooperASC/cooperasc.github.com). Simply sign into your Github account. Non student council members can also use Prose to make changes and submit them for review by a student council member.

### Best practices for file naming

Note URLs should follow this format:

    /_posts/YYYY-MM-DD-event-title-firstname.md
    
- lowercase
- multiple words seperated by dashes
- unneccesary words like "meeting" omitted for brevity

### Ordering posts

Posts in Jekyll are displayed in chronological order according to the date in the post's filename `YYYY-MM-DD-Title.md`. Posts which do not follow this naming convention will not appear on the site. 

    |- /notes
       |- 2012-10-23-student-council.md
       |- 2012-10-24-academic-standards.md
       
### Ordering non-chronological posts

Even posts in sections of the site such as `/people` which aren't necessarily ordered chronologically must be named in this date-like format, however you can "hack" the format, as shown below, to control the display order:

    |- /people
       |- 0100-01-01-casey-gollan.md
       |- 0100-01-02-rachel-appel.md
       |- 0100-01-03-jamshed-bharucha.md

### Adding People

To add a new person, create a file in `/_posts/people/` titled `0100-01-XX-Firstname-Lastname.md`. The required YAML Front Matter is as follows:

    ---
    category: people
    layout: people-single
    title: Jamshed Bharucha
    class: Senior
    email: president@cooper.edu
    published: true
    committees:
    - name: Board Chairman
      link: /committees/#board_chairman
    - name: Web and Social
      link: /committees/#web_and_social
    ---

## Notifications

You can get text notifications when things change by texting "Follow CooperASC" to 40404