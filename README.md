# How to publish a course on FAUN

**TL;DR:**

Publishing a course on FAUN is as easy as writing markdown with some simple rules. Host your course on GitHub, GitLab, or BitBucket, add markdown files with proper headings, include images (png and jpg) in the "images" folder (or a folder of your choice), create a `main.yaml` file in the root of your repository to specify the course files, zip all the files together, and upload the zip file on FAUN to publish your course and start selling it.

## 1. Use GitHub, GitLab, or BitBucket to host your course or work locally

Create a new repository or clone this one locally.

## 2. Add your markdown files

Add your markdown files to the repository (or the folder of your choice if you're not using version control).

For example:

- chapter_1.md
- chapter_2.md
- chapter_3.md
- chapter_4.md
- chapter_5.md

All your content can be also in a single markdown file.

**Notes**:

**1 - Every markdown file must start with a heading. For example:**

✅ Good example (starting with heading level 1 and possibly followed by heading level 2 then 3 and so on):

```markdown
$> cat chapter_1.md

# Chapter 1

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

## Section 1

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
```

❌ Bad example (missing heading level 1 = not valid):

```markdown
$> cat chapter_1.md

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
```

❌ Bad example (missing heading level 1 = not valid):

```markdown
$> cat chapter_1.md

## Chapter 1

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
```

**2 - Every markdown file name should end with the `.md` extension. **

✅ Good example:

```markdown
$> ls 

chapter_1.md
chapter_2.md
chapter_3.md
chapter_4.md
chapter_5.md
```

❌ Bad example:

```markdown
$> ls

chapter_1
chapter_2
chapter_3
chapter_4
chapter_5
```

## 3. Add your images

At the moment, only images are supported (png and jpg). You can add images to your course by adding them to the `images` folder or a folder name of your choice.

## 4. Add your main.yaml file

Make sure you have a `main.yaml` file in the root of your repository. This file contains the course files to parse:

✅ Good example:

```yaml
$> cat main.yaml

---
chapters:
    - chapter_1.md
    - chapter_2.md
    - chapter_3.md
    - chapter_4.md
    - chapter_5.md
```

❌ Bad example:

```yaml
$> cat main.yaml

---

- chapter_1.md
- chapter_2.md
- chapter_3.md
- chapter_4.md
- chapter_5.md
```

## 5. Zip and upload your course

Create a zip files including all your markdown files, images, and the `main.yaml` file. Then, go to [FAUN](https://faun.dev) and upload your course.

Make sure that your files are in the root of the zip file.

✅ Good example:

```bash
course.zip
├── main.yaml
├── chapter_1.md
├── chapter_2.md
├── chapter_3.md
├── chapter_4.md
├── chapter_5.md
├── images
│   ├── image_1.png
│   ├── image_2.png
│   ├── image_3.png
│   ├── image_4.png
```

❌ Bad example:

```bash
course.zip
├── course_files
│   ├── main.yaml
│   ├── chapter_1.md
│   ├── chapter_2.md
│   ├── chapter_3.md
│   ├── chapter_4.md
│   ├── chapter_5.md
│   ├── images
│   │   ├── image_1.png
│   │   ├── image_2.png
│   │   ├── image_3.png
│   │   ├── image_4.png
```

## 6. That's it 🎉

That's it! Your course will be published on FAUN in a few minutes.
