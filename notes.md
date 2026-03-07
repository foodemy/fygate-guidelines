---
title: Markdown Style Guide
description: Standards for creating markdown notes in fyGATE study materials
author: fyGATE
date: 2026-03-04
---

# Markdown Style Guide for fyGATE Study Materials

This document defines the standards for creating markdown notes in this repository.

---

## Frontmatter

Every file must begin with a YAML frontmatter block. This metadata helps with organization, search, and rendering.

### Required Format

```yaml
---
title: Topic Name - Part Number
syllabus:
  - Syllabus 1 covered
  - Syllabus 2 covered
  - Syllabus 3 covered
subject: food-technology
chapter: carbohydrates
part: 1
module: 1
videos:
  - url-1
  - url-2
updatedOn: YYYY-MM-DD
---
```

### Field Descriptions

| Field       | Required | Description                                            |
| ----------- | -------- | ------------------------------------------------------ |
| `title`     | Yes      | Full title of the topic including part number (if any) |
| `syllabus`  | Yes      | Array of topics/concepts covered in the file           |
| `subject`   | Yes      | Parent subject folder name (e.g., `food-technology`)   |
| `chapter`   | Yes      | Topic/chapter name without part number                 |
| `part`      | No       | Part number if topic spans multiple files              |
| `module`    | Yes      | Module number where the topic belongs                  |
| `videos`    | Yes      | URL(s) of the related video lecture(s)                 |
| `updatedOn` | Yes      | Creation or last major update date in `YYYY-MM-DD`     |

### Example Frontmatter

```yaml
---
title: Carbohydrates - 1
syllabus:
  - Introduction to carbohydrates
  - Classification of carbohydrates
  - Structure of monosaccharides
  - Nomenclature of monosaccharides
subject: food-technology
chapter: carbohydrates
part: 1
module: 1
videos:
  - https://youtube.com/watch?v=abc123
  - https://youtube.com/watch?v=def456
updatedOn: 2026-03-03
---
```

### Guidelines

- `syllabus` should list all major topics/concepts covered (one item per topic)
- Use lowercase with hyphens for `subject` and `chapter` (match folder names)
- `videos` must be an array, even for a single video URL
- Update `updatedOn` when making significant content changes
- `module` should match the module number from the course structure

---

## File Organization

### Directory Structure

```yaml
subject-name/
├── topic-name-1/
│   ├── topic-name-1.md
│   └── image1.png
├── topic-name-2/
│   └── topic-name-2.md
```

- Each topic resides in its own folder
- Folder name matches the markdown file name (without extension)
- Images and supplementary files are stored alongside the main markdown file
- Use lowercase with hyphens for folder/file names (e.g., `first-law-of-thermodynamics-2`)

---

## Document Structure

### 1. Title

```markdown
# Carbohydrates - 1
```

- Use H1 (`#`) for the main title only
- Include a part/section number if the topic spans multiple files (e.g., `- 1`, `- 2`)

### 2. Main Content Sections

Use H2 (`##`) for primary sections:

```markdown
## Introduction

## Classification of Carbohydrates

## Structure of Monosaccharides

## Nomenclature
```

### 3. Subsections

Use H3 (`###`) and H4 (`####`) for nested content:

```markdown
### Based on Number of Sugar Units

#### Monosaccharides

Content here...

#### Disaccharides

Content here...
```

---

## Formatting Standards

### Text Formatting

| Element               | Format                 | Example                              |
| --------------------- | ---------------------- | ------------------------------------ |
| Key terms (first use) | Bold                   | **monosaccharides**                  |
| Technical terms       | Bold                   | **glycosidic bond**                  |
| Chemical formulas     | Inline math            | $C_6H_{12}O_6$, $C_{12}H_{22}O_{11}$ |
| Units                 | Plain text after value | 180 g/mol                            |
| Temperatures          | With unit symbol       | 25 °C, 298 K                         |

### Definitions

When introducing a technical term or concept, provide its definition in a blockquote immediately after the paragraph where it first appears.

**Syntax:**

```markdown
Carbohydrates are classified based on the number of sugar units they contain. The simplest carbohydrates are **monosaccharides**.

> **Monosaccharides**: Simple sugars that cannot be hydrolyzed into smaller carbohydrate units. Examples include glucose, fructose, and galactose.

Monosaccharides can combine to form more complex carbohydrates through **glycosidic bonds**.

> **Glycosidic bond**: A covalent bond that joins a carbohydrate molecule to another group, which may or may not be another carbohydrate.
```

**Guidelines:**

- Place the definition blockquote immediately after the paragraph introducing the term
- Start with the term in bold followed by a colon
- Keep definitions concise (1-2 sentences)
- Include examples where helpful
- Only define terms that are essential or may be unfamiliar to the students

### Lists

**Numbered lists** for sequential processes or steps:

```markdown
1. **Glucose**
   - Type: Aldohexose
   - Formula: $C_6H_{12}O_6$
   - Function: Primary energy source for cells
```

**Bullet lists** for non-sequential items:

```markdown
- Monosaccharides
- Disaccharides
- Polysaccharides
```

### Tables

Use tables for summarizing information:

```markdown
| **Carbohydrate** | **Type**       | **Formula**          | **Source**    |
| ---------------- | -------------- | -------------------- | ------------- |
| Glucose          | Monosaccharide | $C_6H_{12}O_6$       | Fruits, honey |
| Sucrose          | Disaccharide   | $C_{12}H_{22}O_{11}$ | Sugarcane     |
```

- Bold the header row content
- Include chemical formulas in math mode within cells

---

## Mathematical Content

### Inline Equations

Use single dollar signs for inline math:

```markdown
The molecular formula of glucose is $C_6H_{12}O_6$ with a molar mass of 180 g/mol.
```

### Block Equations

Use double dollar signs for standalone equations:

```markdown
$$
C_6H_{12}O_6 + 6O_2 \rightarrow 6CO_2 + 6H_2O + \text{Energy}
$$
```

### Multi-line Equations

Use `align*` environment for step-by-step calculations:

```markdown
$$
\begin{align*}
\text{Molar mass of glucose} &= 6(12) + 12(1) + 6(16) \\
&= 72 + 12 + 96 \\
&= 180\ g/mol
\end{align*}
$$
```

### Equation Formatting Guidelines

- Use `\times` for multiplication (not `*` or `x`)
- Use `\frac{numerator}{denominator}` for fractions
- Use `\rightarrow` for reaction arrows
- Use subscripts for chemical formulas: `C_6H_{12}O_6`
- Use `\text{}` for text within equations
- Add `\ ` (backslash-space) before units: `= 180\ g/mol`

### Multi-line Equations Inside Blockquotes

When writing solutions inside blockquotes (for Examples or Previous Years' Questions), multi-line equations require special handling. Each line of the equation block must be prefixed with `>`.

**Syntax:**

```markdown
> **Solution:**
>
> Step explanation here.
>
> $$
> \begin{align*}
> \text{Molar mass} &= 12(12) + 22(1) + 11(16) \\
> &= 144 + 22 + 176 \\
> &= 342\ g/mol
> \end{align*}
> $$
>
> Therefore, the molar mass of maltose is **342 g/mol**.
```

**Key Points:**

- Every line inside the blockquote (including blank lines within `$$`) must start with `>`
- Leave a blank `>` line before and after the equation block for proper rendering
- The `$$` delimiters must also be on their own lines with `>` prefix
- Ensure no trailing spaces after `>` on blank lines

---

## Images

Use HTML `<figure>` elements for images with captions to ensure proper rendering and centering on GitHub.

**Syntax:**

```markdown
<figure>
  <img src="glucose-structure.png" alt="Structure of glucose molecule showing the ring form">
  <figcaption>Figure 1: Structure of glucose in its cyclic form</figcaption>
</figure>
```

**Guidelines:**

- Use descriptive filenames: `glucose-structure.png`, `glycosidic-bond.png`
- Store images in the same folder as the markdown file
- Provide meaningful alt text that describes the image content
- Include a caption using `<figcaption>` to explain the figure
- Use PNG format for diagrams, JPG for photographs
- Number figures sequentially within each document (Figure 1, Figure 2, etc.)

---

## Examples Section

### Structure

```markdown
---

## Examples

### Example 1

Calculate the molar mass of maltose ($C_{12}H_{22}O_{11}$).

> **Solution:**
>
> Maltose has the molecular formula $C_{12}H_{22}O_{11}$
>
> $$
> \begin{align*}
> \text{Molar mass} &= 12(12) + 22(1) + 11(16) \\
> &= 144 + 22 + 176 \\
> &= 342\ g/mol
> \end{align*}
> $$
```

### Guidelines

- Separate Examples section from main content with horizontal rule (`---`)
- Number examples sequentially: `### Example 1`, `### Example 2`
- Write problem statement in plain text (not blockquote)
- Place entire solution inside a blockquote (`>`)
- Show all intermediate steps with equations
- State the final answer clearly with appropriate units

---

## Practice Questions Section

### Structure

```markdown
---
## Practice Questions

### Question 1

Classify the following carbohydrates and write their molecular formulas:
  - (i) Glucose
  - (ii) Sucrose
  - (iii) Starch
---

### Question 2

Explain the difference between alpha and beta glycosidic bonds.

> Hint:
>
> - Consider the orientation of the -OH group at C1
> - Think about how this affects digestibility
```

### Guidelines

- Separate from Examples with horizontal rule
- Number questions sequentially
- Use roman numerals for multi-part questions: `(i)`, `(ii)`, `(iii)`
- Place supplementary data or hints in blockquotes
- Separate individual questions with horizontal rules (`---`)

---

## Solutions Section

### Structure

```markdown
---
## Solutions

### Question 1

(i) **Glucose** - Monosaccharide, $C_6H_{12}O_6$

(ii) **Sucrose** - Disaccharide, $C_{12}H_{22}O_{11}$

(iii) **Starch** - Polysaccharide, $(C_6H_{10}O_5)_n$
---

### Question 2

...
```

### Guidelines

- Match question numbering exactly
- Do NOT use blockquotes (to differentiate from example solutions)
- Show complete working with all steps
- Separate solutions with horizontal rules

**Important:** Practice Question solutions must be in a **separate Solutions section**, NOT inline with the questions. This keeps the Practice Questions section clean for self-assessment — students can attempt questions without accidentally seeing answers.

---

## Previous Years' Questions Section

### Structure

```markdown
---

## Previous Years' Questions

### Question 1 (GATE 2023)

Which of the following is a reducing sugar?

- (A) Sucrose
- (B) Maltose
- (C) Trehalose
- (D) None of the above

> **Solution:**
>
> Maltose is a reducing sugar because it has a free anomeric carbon that can act as a reducing agent.
>
> **Answer: (B)**

---

### Question 2 (GATE 2021)

The glycosidic bond in cellulose is: #GATE2021

- (A) α-1,4
- (B) β-1,4
- (C) α-1,6
- (D) β-1,6

> **Solution:**
>
> Cellulose consists of glucose units linked by **β-1,4 glycosidic bonds**.
>
> **Answer: (B)**
```

### Guidelines

- Include exam name and year in heading: `### Question 1 (GATE 2023)`
- For MCQs/MSQs, list options with `(A)`, `(B)`, `(C)`, `(D)` format
- Place solutions in blockquotes
- Separate questions with horizontal rules

---

## Section Order

Maintain this order in all notes:

1. **Frontmatter** (YAML metadata block)
2. Title
3. Main content sections (theory, classification, structure, etc.)
4. `---`
5. Examples (with solutions in blockquotes)
6. `---`
7. Practice Questions
8. `---`
9. Solutions
10. `---`
11. Previous Years' Questions

---

## Checklist Before Committing

- [ ] Frontmatter present with all required fields (`title`, `description`, `subject`, `chapter`, `module`, `videos`, `updatedOn`)
- [ ] File and folder names use lowercase with hyphens
- [ ] H1 used only for main title
- [ ] All equations render correctly (test in preview)
- [ ] Images have width specified and files exist
- [ ] Examples have solutions in blockquotes
- [ ] Practice question solutions are NOT in blockquotes
- [ ] Previous years' questions include exam name and year
- [ ] Horizontal rules separate major sections
- [ ] All variables use consistent notation throughout
- [ ] Units are included with all numerical answers
