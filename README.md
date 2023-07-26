# How to publish a course on FAUN

Publishing a course on FAUN is as easy as writing markdown with some simple rules. Here are some simple steps to get you started.

## 1. Use GitHub, GitLab, or BitBucket to host your course (optional)

Create a new repository or clone this one.

## 2. Add your markdown files

Add your markdown files to the repository. For example:

- chapter_1.md
- chapter_2.md
- chapter_3.md
- chapter_4.md
- chapter_5.md

You can add everything to a single file, or you can add each chapter to a separate file.

**Notes**:

1 - Every markdown file must start with a heading. For example:

```markdown
# Chapter 1
```

2 - Every markdown file name should end with the `.md` extension. 

```markdown
chapter_1.**md**
```

## Add your images

At the moment, only images are supported (png and jpg). You can add images to your course by adding them to the `images` folder or a folder name of your choice.

## Add your main.yaml file

Make sure you have a `main.yaml` file in the root of your repository. This file contains the course files to parse:

```yaml
content:
    - chapter_1.md
    - chapter_2.md
    - chapter_3.md
    - chapter_4.md
    - chapter_5.md
```

## Zip and upload your course

Create a zip files including all your markdown files, images, and the `main.yaml` file. Then, go to [FAUN](https://faun.dev) and upload your course.

Make sure that your files are in the root of the zip file.

Good example:

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

Bad example:

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

## That's it 🎉

That's it! Your course will be published on FAUN in a few minutes.
