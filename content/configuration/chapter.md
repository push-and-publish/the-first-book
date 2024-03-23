# Configuration

The book.yml file in your repository's main directory is the center of the book configuration. It contains the book name, chapters, optional dedication text, and cover image path.

## Chapters configuration

If you will use the following chapter configuration:

```yaml
name: 'My first book'
chapters:
  - name: Introduction
    slug: introduction
```

The tool will look for a `content/introduction/chapter.md` file. As you may already noticed, the `slug` attribute is the directory's name in the repository, while the `name` attribute will be used inside the book in the table of contents section.

### Chapters order

The order of chapters definitions is important because the same order will be used during rendering. In the below example, the Introduction chapter will be rendered before the Afterword chapter.

```yaml
name: 'My first book'
chapters:
  - name: Introduction
    slug: introduction
  - name: Afterword
    slug: afterword
```
