# Self-solve quiz

An example physics quiz for students.

## Setup

### Tolerance

`defaultTolerance` defines the tolerance used if a question doesn't define its
own tolerance.

### How many questions

`numberOfQuestions` - this many questions are picked at random from the list.

## Making changes to questions

At the top of the page is a script tag including the question data, it's
expected to be of the form:

```
{
  title: "Question title",
  description: "HTML description of the problem",
  inputLabel: "Label for the input field",
  correctAnswer: 4.17,
  tolerance: 0.0001,
  correctLaw: "B",
  solution: `Step-by-step solution
  can be on multiple lines`
}
```

_(Any of the strings can be multiple lines using backticks (`).)_

The `tolerance` key is optional - if not provided the `defaultTolerance`, also
defined in the top script block, will be used.

## Testing locally

Download `body-only.html` save it to a file with the `.html` extension and open
it. It should just-work, if it does not you can open the file by typing in your
browser location bar `file:/// .... path to /body-only.html`.

Note that the file is incomplete (has no `head` or `body`) so browsers may warn
about this, but it doesn't matter because that's not how this content is going
to be used.

## Uploading to exe learning

* Multiple steps of hoop jumping
* Click on the code view in the WYSIWYG editor
* Paste the whole contents of `body-only.html`
* Ignore it being shown as blank
* Save
* More hoop-jumping to preview the page
