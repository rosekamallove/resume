# resume.md

<!-- ![Resume](resume.png) -->

Write your resume in
[Markdown](https://raw.githubusercontent.com/mikepqr/resume.md/main/resume.md),
style it with [CSS](resume.css), output to [HTML](resume.html) and
[PDF](resume.pdf).

## Prerequisites

- Python ≥ 3.6
- [python-markdown](https://python-markdown.github.io/) (`pip install markdown`)
- Optional, required for PDF output: Google Chrome or Chromium

## Usage

1.  Download [resume.py](resume.py), [resume.md](resume.md) and
    [resume.css](resume.css) (or make a copy of this repository by [using the
    template](https://github.com/mikepqr/resume.md/generate), forking, or
    cloning).

2.  Edit [resume.md](resume.md) (the placeholder text is taken with thanks from
    the [JSON Resume Project](https://jsonresume.org/themes/))

3.  Run `python3 resume.py` to build resume.html and resume.pdf.

    - Use `--no-html` or `--no-pdf` to disable HTML or PDF output.

    - Use `--chrome-path=/path/to/chrome` if resume.py cannot find your Chrome
      or Chromium executable.

## Customization

Edit [resume.css](resume.css) to change the appearance of your resume. The
default style is extremely generic, which is perhaps what you want in a resume,
but CSS gives you a lot of flexibility. See, e.g. [The Tech Resume
Inside-Out](https://www.thetechinterview.com/) for good advice about what a
resume should look like (and what it should say).

Change the appearance of the PDF version (without affecting the HTML version) by
adding rules under the `@media print` CSS selector.

Change the margins and paper size of the PDF version by editing the [`@page` CSS
rule](https://developer.mozilla.org/en-US/docs/Web/CSS/%40page/size).

[python-markdown](https://python-markdown.github.io/) is by default a very basic
markdown compiler, but it has a number of optional extensions that you may want
to enable (by adding to [the list of extensions
here](https://github.com/mikepqr/resume.md/blob/5d99e02bf65ff6a2a0ccd18c1a0255c26ec59377/resume.py#L41)).
<code><a
href="https://python-markdown.github.io/extensions/attr_list/">attr_list</a></code>
in particular may by useful if you are editing the CSS.

### STAR Method for better bullet points:

The STAR method can help you create impactful descriptions for each experience on your resume.

**Situation:** What was the situation, problem, or conflict you were facing?

**Task:** What were you tasked with? What were your responsibilities or goals?

**Action:** What action did you take? What did you do to solve this problem? (start with action verbs)

**Result:** What was the result or outcome of your action? How did it benefit the organization? Can this result be quantified?

#### Example

Skills/qualities you want to show: initiative, organization, analytical thinking, writing, interpersonal skills, problem solving

Situation: The trainees were learning too slowly and could not navigate the company’s data tracking system by the end of the two-week training period. Instead, they were not ready for another two weeks.

Task: Help trainees learn the system faster.

Action: Initiated, wrote, and edited the first training manual for the company’s data tracking system. Successfully presented proposal to use manual to management. Revised training program curriculum to implement new manual. Trainees worked through the manual during the two-week training period.

Result: At the end of the training period, trainees were ready to use the data tracking system two weeks earlier than expected; the training manual was adopted across the company and is still in use.

FINAL STATEMENT FOR RESUME: Initiated, wrote, and edited the first training manual for company’s data tracking system, which cut training period in half, was adopted across the company, and is still in use today.

This example could focus on different skills (communication, persuasion, leadership, training), depending on what’s relevant to the job.
