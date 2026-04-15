# How to Create a Mini Table of Contents for Each Chapter in Word

This guide explains how to create a **mini table of contents** at the beginning of each chapter in Microsoft Word, like the one shown in your example.

---

## 1. Use heading styles properly

Apply Word’s built-in heading styles consistently:

- **Heading 1** → chapter title  
  Example: `Chapter 1`, `Introduction`
- **Heading 2** → section titles  
  Example: `1.1 Architecture Overview`
- **Heading 3** → subsection titles, if needed

This is necessary because Word generates tables of contents from heading styles.

---

## 2. Put each chapter on its own opening page

At the start of each new chapter:

1. Insert a **Page Break**
2. Type the chapter heading
3. Type the chapter title underneath

This creates a clean chapter-opening page.

---

## 3. Bookmark the whole chapter

This is the key step for creating a chapter-specific mini TOC.

### Steps:
1. Select the entire chapter content, from the chapter title down to just before the next chapter
2. Go to **Insert → Bookmark**
3. Give it a name such as:
   - `ch1`
   - `ch2`
   - `ch3`
4. Click **Add**

Repeat this for every chapter.

---

## 4. Insert the mini table of contents

Place the cursor where you want the mini TOC to appear.

### Insert the field:
Press:

**Ctrl + F9**

Word will insert field braces:

```text
{TOC \o "2-3" \h \z \b ch1 }
```
Then:
Right-click the field
Choose Update Field

This will generate a TOC:

only for the bookmarked chapter (ch1)
only for Heading 2 and Heading 3
so the mini TOC will show entries such as:
1.1 Architecture Overview
1.2 Thesis Structure

and not the main chapter title.

Example for other chapters:

Chapter 1:

{ TOC \o "2-3" \h \z \b ch1 }

Chapter 2:

{ TOC \o "2-3" \h \z \b ch2 }

5. Add the horizontal lines

To create the top and bottom lines around the mini TOC:

Option A: Use paragraph borders
Place the cursor above the mini TOC
Go to Home → Borders
Apply a Top Border or Bottom Border
Option B: Use lines as shapes
Go to Insert → Shapes → Line
Draw the line above and below the mini TOC