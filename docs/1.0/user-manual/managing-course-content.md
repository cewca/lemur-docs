# Managing course content

## Structure of a Lemur course

Courses in Lemur Learning are structured as a series of ordinary web pages,
with a persistent sidebar for the table of contents, and a page-specific
comments area at the foot of each page.

Learners are free to jump between pages and work in any order they choose,
and their progress will  be tracked in the sidebar under the table of
contents, to help ensure they complete the necessary requirements for
the course.

How you direct your learners from activity to activity relies mainly on
how you structure your course content. Activities can be separated between
pages, or they can appear one after another on a single page. Lemur leaves
that completely in your control as a content author.

Longer pages can be daunting for some learners, while the "one activity
per page" approach can create a long table of contents and a lot of extra
clicking between pages.

From our experience, the best balance is somewhere in between. By
combining related content and activities on a single page, it can be
easier for learners to see the connections between concepts.

## The page editor

The page editor is found under the `Pages` link next to a course under
the Tools > Courses screen. Click on the `Content` link next to a page
to open the page editor for that page, or click `Add Page` and choose
a page name to bring up the page editor for a new page.

> Tip: To reorder the pages in your course, drag and drop them into the order
you want on the page list screen.

The page editor has two columns. On the left is a list of objects that
can be added to the page. This includes content like text, images and
video, as well as learner inputs for building quizzes and assessments.

The right column contains the page content as a series of content
objects. In the top right of the page content are tabs to switch
between three views of the content: Edit, Sort, and Preview.

Here is a screenshot of the page editor:

![Lemur Learning page editor](/apps/docs/docs/1.0/pix/page-editor.png)

Click on an object type to add it to the page. Switch to the Sort
tab to reorder objects within the page, and switch to Preview to see
how they will look in the course itself.

> Note: Changes made in the page editor are automatically saved in the background
as you work.

## Sections and quizzes

There are two special objects that group related content together.
These are the `Section` and `Quiz` objects.

Both have the effect of adding a section link under the page link in
the table of contents, which can be used to add further structure to
a course.

The `Quiz` object has the additional effect that any learner inputs
directly following will be converted into a single quiz that must
be submitted all together instead of answering each question
separately.

This lets you add single questions throughout your course to encourage
critical thinking, as well as longer inputs for more in-depth assessment,
for example at the end of a chapter.

## Page comments

In developing Lemur Learning, we experimented with a number of forms of
learner-to-learner dialogue before making page-specific comments the
default mode of communication between learners.

Compared to course-wide forums, we found that forums separated the
learner-generated content from the original course content, removing
valuable context for future learners by making it harder to cross-reference.

We also experimented with realtime chat within courses, but found that
chat would only be used when a significant number of learners were
present at the same time, and when learners saw that there was no one
else online they seldom came back to the chat after that. We also found
that chat archives make for a poor format for future learners to
learn from.

Comments on the other hand are attached directly to the page they're
referencing, so context is maintained, and that also encourages
participation even when learners aren't all online together. There's
also a wiki-like quality to comments, where they become a living part
of the course content over time.

See the [[:Managing discussions]] page for more info about managing
comments in your courses.

> Note: If shared learner comments are not appropriate for your site, you can disable
commenting under Tools > Courses > Settings.

Next: [[:Managing learners]]