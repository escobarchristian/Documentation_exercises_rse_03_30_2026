# Documentation for Research Software

A complete 1-hour-20-minute class on writing documentation for research software projects. Designed for a research software engineering course where students may not have formal software development training.

## Overview

Researchers write code every day, but that code is often undocumented, difficult to reuse, and impossible to understand six months later. This class teaches students **why** documentation matters and **how** to write it at every level — from inline comments to full project READMEs — through a mix of lecture slides, live examples, and hands-on exercises in Google Colab.

By the end of this class, students will be able to:

- Explain the difference between a comment and a docstring
- Write Google-style docstrings with Args, Returns, Raises, and Examples
- Create a README with installation instructions, a quick-start example, and a citation
- Give constructive code review feedback that improves documentation quality

## Repository Contents

```
├── documentation_slides.pptx          # Lecture slides (17 slides)
├── presenter_script.md                # Slide-by-slide talking points and timing
├── examples.ipynb                     # Demo notebook: docstrings, pydoc, and Markdown
├── exercises/
│   ├── exercise_1_mystery_functions.ipynb   # Rename and document bad functions
│   ├── exercise_2_readme.ipynb              # Fill in a README template
│   └── exercise_3_code_review.ipynb         # Write constructive review comments
├── solutions/
│   ├── exercise_1_solutions.ipynb
│   ├── exercise_2_solutions.ipynb
│   └── exercise_3_solutions.ipynb
└── README.md
```

## How to Use This Material

### For instructors

1. **Before class:** Review the [presenter script](presenter_script.md) to familiarize yourself with the flow and timing. The script includes suggested pacing, discussion prompts, and notes on where students tend to engage most.

2. **During the lecture (~55 min):** Present the [slides](documentation_slides.pptx). The deck is structured as follows:

   | Slides | Topic | Time |
   |--------|-------|------|
   | 1 | Title | ~1 min |
   | 2 | Why documentation matters | ~3 min |
   | 3 | Four levels of documentation | ~2 min |
   | 4–5 | Bad vs. good code example (interactive) | ~7 min |
   | 6–8 | Docstrings: definition, anatomy, formats | ~9 min |
   | 9 | Comments and docstrings best practices | ~3 min |
   | 10 | README files | ~3 min |
   | 11 | Diátaxis framework (Tutorials, How-Tos, Explanation, Reference) | ~3 min |
   | 12–13 | API documentation and tooling | ~4 min |
   | 14 | Documentation as workflow | ~4 min |
   | 15–16 | Code review and giving constructive feedback | ~9 min |
   | 17 | Q&A | ~5 min |

3. **During the exercises (~25 min):** Have students open the exercise notebooks in Google Colab. They are designed to be completed in order, roughly 8 minutes each. Share the solution notebooks after students have finished.

4. **Optionally:** Walk through the [demo notebook](examples.ipynb) live to show `help()`, `pydoc`, and Markdown rendering in Colab before students start the exercises.

### For students

All exercises run in **Google Colab** — no installation required. Click the links your instructor provides, or upload the `.ipynb` files to [colab.research.google.com](https://colab.research.google.com).

## Exercises

### Exercise 1 — Fix the Mystery Functions

Two short functions with bad names and no documentation. Students run them, figure out what they do, then rewrite them with descriptive names, type hints, and Google-style docstrings. The first function includes a fill-in-the-blank template; the second asks students to write from scratch.

**Concepts practiced:** naming, type hints, docstring structure, `help()`

### Exercise 2 — Write a README

Students fill in a README template for a simple project (a grade calculator script). The template provides the structure with blank fields to complete, so students focus on content rather than formatting.

**Concepts practiced:** README sections (purpose, installation, usage, license), Markdown syntax

### Exercise 3 — Code Review Practice

Students review a short function with obvious issues (vague names, no docstring, a `print()` side effect) and write three constructive comments using sentence starters. This reinforces both documentation skills and the feedback guidelines from the lecture.

**Concepts practiced:** constructive feedback, identifying documentation gaps, code review tone

## Topics Covered

### Level 1 — Comments and Docstrings
- What a docstring is and how Python stores it in `__doc__`
- The difference between comments (`#`) and docstrings (`"""`)
- Anatomy of a Google-style docstring (summary, Args, Returns, Raises, Example)
- Google vs. NumPy docstring formats and when to use each

### Level 2 — README Files
- The six sections every README needs: project purpose, installation, quick start, configuration, citation, and license
- Writing for someone who has never seen your project

### Level 3 — Guides and Tutorials
- The Diátaxis framework: tutorials, how-to guides, explanation, and reference
- When a project outgrows a README

### Level 4 — API Reference Documentation
- Auto-generating docs from docstrings with Sphinx, MkDocs, and pdoc
- The write → build → publish pipeline

### Documentation Workflow
- Docs-as-code: keeping documentation in the repository
- Writing documentation alongside code, not after
- CHANGELOG, CITATION.cff, and data documentation

### Code Review
- The Who / What / When / Why framework for collaborative construction
- Giving feedback that people will actually listen to
- Criticize the code, not the coder

## Prerequisites

- Basic Python knowledge (functions, lists, loops)
- A Google account (for Colab access)
- No software installation required

## Acknowledgments

The code review material draws on the [INTERSECT Code Review training module](https://intersect-training.org/Code-Review/introduction.html), licensed under CC-BY 4.0.

## License

This material is available under the [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) license. You are free to share and adapt it for any purpose, provided you give appropriate credit.
