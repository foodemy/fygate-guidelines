---
title: Style Guide
description: Standards for styles used in fyGATE study materials
author: fyGATE
updatedOn: 2026-03-11
---

# Style Guide for fyGATE Study Materials

This document defines the writing style, language conventions, and content standards for all fyGATE study materials.

---

## Language Standards

### British English

All content must be written in **British English**. This applies to spelling, grammar, and terminology.

| American English | British English |
| ---------------- | --------------- |
| color            | colour          |
| flavor           | flavour         |
| organize         | organise        |
| analyze          | analyse         |
| fiber            | fibre           |
| center           | centre          |
| liter            | litre           |
| meter            | metre           |
| labeled          | labelled        |
| modeling         | modelling       |

**Examples:**

- ❌ "The color of the solution changed..."
- ✅ "The colour of the solution changed..."

- ❌ "Analyze the following data..."
- ✅ "Analyse the following data..."

- ❌ "The fiber content was measured..."
- ✅ "The fibre content was measured..."

---

## Writing Style

### Bullet-Point Approach

fyGATE study materials use a **bullet-point-first approach** instead of traditional paragraphs. Each concept, fact, or piece of information is written as a separate bullet point. This makes content:

- Easier to scan and review
- Better for quick revision
- More suitable for digital note-taking

### Tone and Voice

- Use a **formal but accessible** tone
- Write in **third person** for theoretical content
- Avoid colloquialisms and informal expressions

**Examples:**

- ❌ "You'll find that glucose is pretty important..."
- ✅ "Glucose plays a crucial role in cellular metabolism."

- ❌ "This stuff is super reactive..."
- ✅ "This compound exhibits high reactivity."

### Sentence Structure Within Bullets

- Each bullet should be a complete, meaningful sentence
- Keep sentences clear — avoid overly complex structures
- Use active voice when appropriate
- One main idea per bullet point

---

## Bullet Points and Lists

### Primary Content Format

Bullet points are the **primary format** for all theoretical content in fyGATE notes. Each bullet should convey a complete thought that can stand on its own.

**Example — Food Pigments Topic:**

```markdown
- Food pigments are naturally occurring compounds present in plant and animal tissues. They impart colour to the cells in which they exist.
- They play a very important role in enhancing the aesthetic appearance of foods.
- Pigments are technically chemical compounds that absorb light in the wavelength range of the visible region.
- The colour produced by a pigment depends on a specific part of its molecule called the **chromophore**. When light strikes this structure, it absorbs certain wavelengths of light, causing electrons to jump to a higher energy level (excitation). The wavelengths of light that are not absorbed are reflected or refracted back; these are detected by our eyes and interpreted as colour.
- Pigments extracted from plants, animals, and minerals have been widely used for imparting colour to various foods. Nowadays, use of synthetic dyes is also more common.
- Various natural pigments found in food sources include:
  - Chlorophylls
  - Myoglobin and haemoglobin
  - Anthocyanins
  - Carotenoids
  - Flavonoids
  - Tannins
  - Betalains
  - Quinones and xanthones
```

### Guidelines for Writing Bullet Points

1. **One concept per bullet** — Each bullet should focus on a single idea or closely related ideas
2. **Complete sentences** — Write full sentences, not fragments (unless in a sub-list)
3. **Logical flow** — Arrange bullets in a logical sequence (introduction → details → examples)
4. **Self-contained** — Each bullet should make sense on its own without needing context from other bullets
5. **Appropriate length** — Bullets can be multiple sentences if they explain a single concept

### When to Use Sub-Bullets

Use sub-bullets (nested lists) for:

- Listing examples, types, or categories
- Breaking down components of a concept mentioned in the parent bullet
- Enumerating items that belong together

**Example:**

```markdown
- Carbohydrates are classified based on the number of sugar units they contain:
  - Monosaccharides (single sugar unit)
  - Disaccharides (two sugar units)
  - Oligosaccharides (3–10 sugar units)
  - Polysaccharides (more than 10 sugar units)
```

### When to Use Numbered Lists

Use numbered lists only for:

- Sequential steps or processes
- Ranked items
- Items that need to be referenced by number

**Example:**

```markdown
The Maillard reaction occurs in three stages:

1. **Initial stage** — Condensation of reducing sugar with amino acid to form Amadori products
2. **Intermediate stage** — Breakdown of Amadori products to form various reactive intermediates
3. **Final stage** — Formation of brown pigments (melanoidins) and flavour compounds
```

### Avoiding Meaningless Bullets

Ensure each bullet adds value. Avoid bullets that are too vague or lack context.

**Poor Example:**

```markdown
- Glucose
- Important
- Energy
- Cells
```

**Good Example:**

```markdown
- Glucose is the primary energy source for cells.
- It is metabolised through glycolysis to produce ATP.
- The brain relies almost exclusively on glucose for its energy needs.
```

### Punctuation in Bullets

- **Full sentences**: End with a full stop
- **Sub-bullets (short phrases/single words)**: No full stop needed
- **Consistency**: Maintain the same punctuation style throughout a section

**Example:**

```markdown
- Starch is the storage polysaccharide in plants.
- It consists of two components:
  - Amylose (linear chain)
  - Amylopectin (branched chain)
- Starch granules are insoluble in cold water but gelatinise when heated.
```

---

## Images and Diagrams

### Originality Requirements

- **Original images are mandatory** — Create diagrams, flowcharts, and illustrations specifically for fyGATE materials
- **No direct copying** — Do not use copyrighted images from textbooks, websites, or other sources without permission
- **Redraw when necessary** — If referencing an existing diagram concept, redraw it using AI tools (Gemini) or design software to create an original version

### Image Creation Workflow

1. Identify the concept that needs visual representation
2. Search for reference images to understand the standard representation
3. Create an original version using:
   - AI image generation tools (e.g., Gemini)
   - Design software (e.g., Canva, draw.io, BioRender)
   - Hand-drawn diagrams (scanned and cleaned)
4. Ensure the image is clear, accurate, and appropriately sized

### Required Image Elements

Every image must include:

1. **Figure number** — Sequential within the document
2. **Caption** — Brief description of what the image shows
3. **Alt text** — Detailed description for accessibility

### Alt Text Explained

**Alt text** (alternative text) is a written description of an image that serves two purposes:

1. **Accessibility** — Screen readers read alt text aloud for visually impaired users
2. **Fallback** — Displays when the image fails to load

**Guidelines for writing alt text:**

- Describe the content and purpose of the image
- Be specific but concise (typically 125 characters or fewer)
- Include relevant details that convey the educational value
- Do not start with "Image of..." or "Picture of..."
- Include text that appears in the image

### Image Syntax

Use HTML `<figure>` elements for proper rendering:

```html
<figure>
  <img
    src="glucose-ring-structure.png"
    alt="Cyclic structure of glucose showing the six-membered pyranose ring with hydroxyl groups at positions 1-4 and 6, and CH2OH group at position 5"
  />
  <figcaption>Figure 1: Cyclic (pyranose) form of D-glucose</figcaption>
</figure>
```

### Examples of Good Alt Text

**Example 1 — Chemical Structure:**

```html
<img
  src="maltose-structure.png"
  alt="Maltose molecule showing two glucose units connected by an alpha-1,4 glycosidic bond, with the free anomeric carbon on the right glucose unit"
/>
```

**Example 2 — Flowchart:**

```html
<img
  src="glycolysis-pathway.png"
  alt="Flowchart of glycolysis showing glucose conversion to pyruvate in 10 steps, with ATP and NADH production indicated at relevant steps"
/>
```

**Example 3 — Graph:**

```html
<img
  src="enzyme-kinetics.png"
  alt="Graph plotting reaction velocity against substrate concentration, showing hyperbolic curve reaching maximum velocity (Vmax) with Km marked at half-Vmax"
/>
```

### Image File Naming

- Use lowercase letters only
- Separate words with hyphens
- Be descriptive but concise
- Include the subject matter

**Examples:**

- ✅ `glucose-ring-structure.png`
- ✅ `starch-amylose-amylopectin-comparison.png`
- ❌ `IMG_2847.png`
- ❌ `Figure1.png`
- ❌ `Glucose Structure.png`

---

## Terminology and Definitions

### Consistent Terminology

- Use the same term for a concept throughout the document
- Define technical terms on first use
- Prefer widely accepted terminology over regional variants

**Example:**

- ❌ Using "simple sugars", "monosaccharides", and "single sugars" interchangeably
- ✅ Define "monosaccharides" once, then use it consistently

### Introducing Technical Terms (Within Bullets)

When introducing a new technical term within the bullet-point format:

1. **Bold** the term on first use within the bullet
2. Provide the definition or explanation in the same bullet or the following bullet
3. Use the term normally thereafter (no bold)

**Example — Inline Definition:**

```markdown
- The colour produced by a pigment depends on a specific part of its molecule called the **chromophore**. When light strikes this structure, it absorbs certain wavelengths of light, causing electrons to jump to a higher energy level (excitation).
```

**Example — Follow-up Definition:**

```markdown
- Sugars that can reduce oxidising agents are called **reducing sugars**.
- Reducing sugars have a free aldehyde or ketone group capable of acting as a reducing agent. Examples include glucose, fructose, and maltose.
- Reducing sugars give a positive result in Benedict's test.
```

### Formal Definitions (Blockquote Format)

For important terms that require a formal, standalone definition, use the blockquote format immediately after the bullet that introduces the term.

**Example:**

```markdown
- The simplest carbohydrates are **monosaccharides**.

> **Monosaccharides**: Simple sugars that cannot be hydrolysed into smaller carbohydrate units. Examples include glucose, fructose, and galactose.

- Monosaccharides can combine to form more complex carbohydrates through glycosidic bonds.
```

**When to use blockquote definitions:**

- Key terms that students must memorise
- Terms likely to appear in exam questions
- Concepts that require precise, textbook-style definitions

---

## Numbers and Units

### Number Formatting

| Type                        | Format               | Example        |
| --------------------------- | -------------------- | -------------- |
| Numbers less than 10        | Spell out            | three, seven   |
| Numbers 10 and above        | Use digits           | 15, 250        |
| Numbers starting a sentence | Always spell out     | Twenty samples |
| Large numbers               | Use commas           | 1,000,000      |
| Decimals                    | Use digits with dot  | 3.14, 0.05     |
| Ranges                      | Use en-dash          | 20–30 °C       |
| Percentages                 | Digit + % (no space) | 95%            |

### Units

- Always include a space between number and unit: `25 °C`, `180 g/mol`
- Use SI units where applicable
- Write unit symbols, not names, after numbers: `5 kg` not `5 kilograms`
- Use superscripts for squared/cubed units: `m²`, `cm³`

**Examples:**

- ❌ "The temperature was 25°C"
- ✅ "The temperature was 25 °C"

- ❌ "Add 500ml of water"
- ✅ "Add 500 mL of water"

### Subscripts and Superscripts in Units

Markdown does not have native support for subscripts or superscripts. Use **LaTeX math mode** to render them.

**Syntax:**

| Element     | LaTeX Syntax | Rendered Output |
| ----------- | ------------ | --------------- |
| Superscript | `$m^2$`      | $m^2$           |
| Subscript   | `$H_2O$`     | $H_2O$          |
| Both        | `$Ca^{2+}$`  | $Ca^{2+}$       |

**Examples:**

```markdown
- The surface area was 25 $m^2$.
- Water ($H_2O$) is essential for life.
- The unit of acceleration is $m/s^2$.
- Calcium ions ($Ca^{2+}$) are important for bone health.
- The concentration was 5 $mg/cm^3$.
```

**Guidelines:**

- Use curly braces `{}` for multi-character subscripts or superscripts: `$C_{12}H_{22}O_{11}$` → $C_{12}H_{22}O_{11}$
- Single characters do not need braces: `$m^2$`, `$O_2$`
- For units within equations, use `\text{}` for non-italicised text: `$5\ \text{kg/m}^3$`

---

## Abbreviations and Acronyms

### First Use

- Spell out the full term on first use, followed by the abbreviation in parentheses
- Use the abbreviation thereafter

**Example:**

"The **Food Safety and Standards Authority of India (FSSAI)** regulates food standards in India. FSSAI guidelines specify..."

### Common Abbreviations

Do not expand universally known abbreviations:

- DNA, RNA, ATP, pH, UV, IR

### Subject-Specific Abbreviations

Always expand on first use:

- HPLC (High-Performance Liquid Chromatography)
- GC-MS (Gas Chromatography-Mass Spectrometry)
- aw (water activity)

---

## Capitalisation

### General Rules

- Capitalise proper nouns (names of people, places, organisations)
- Capitalise the first word after a colon if it begins a complete sentence
- Use sentence case for headings (capitalise first word and proper nouns only)

### Scientific Terms

- **Do not capitalise** general scientific terms: glucose, enzyme, protein
- **Capitalise** terms derived from proper nouns: Maillard reaction, Fehling's test, Benedict's solution
- **Capitalise** genus names but not species: _Saccharomyces cerevisiae_

**Examples:**

- ❌ "The Glucose Molecule is important"
- ✅ "The glucose molecule is important"

- ❌ "The maillard reaction occurs during heating"
- ✅ "The Maillard reaction occurs during heating"

---

## Quotations and Citations

### Direct Quotations

- Use double quotation marks for direct quotes: "..."
- Use single quotation marks for quotes within quotes: '...'
- Place punctuation inside quotation marks (British style allows either, but be consistent)

### Citing Sources

For GATE preparation materials:

- Cite previous year questions with exam name and year: (GATE 2023)
- Reference standard textbooks by author surname: (Fennema, 2017)

---

## Common Errors to Avoid

| Error                     | Incorrect                        | Correct                        |
| ------------------------- | -------------------------------- | ------------------------------ |
| It's vs Its               | "It's structure is complex"      | "Its structure is complex"     |
| Affect vs Effect          | "This will effect the result"    | "This will affect the result"  |
| Comprise vs Compose       | "Starch is comprised of glucose" | "Starch comprises glucose"     |
| Less vs Fewer             | "Less molecules"                 | "Fewer molecules"              |
| Which vs That             | "The enzyme which catalyses..."  | "The enzyme that catalyses..." |
| Data (plural)             | "The data shows..."              | "The data show..."             |
| Different from (not than) | "Different than other sugars"    | "Different from other sugars"  |

---

## Checklist Before Submission

- [ ] British English spelling used throughout
- [ ] Content written in bullet-point format (not paragraphs)
- [ ] Each bullet is a complete, meaningful sentence
- [ ] Technical terms bolded and defined on first use
- [ ] All images are original or redrawn
- [ ] All images have figure numbers, captions, and alt text
- [ ] Numbers and units formatted correctly
- [ ] Abbreviations expanded on first use
- [ ] Consistent terminology throughout
- [ ] No informal language or colloquialisms
- [ ] Grammar and punctuation checked
