# Tutorials

Tutorials are available at [sparrowcode.io/en](https://sparrowcode.io) & [sparrowcode.io/ru](https://sparrowcode.io).
Here you can add a new tutorial, supplement or correct typos in existing tutorials. If you want to help the project, take a look at the [todo](https://github.com/sparrowcode/tutorials/blob/main/TODO.md) list.

## Navigate

- [Contribute](#contribute)
  - [Content](#content)
  - [Formatting](#formatting)
  - [Meta](#meta)
  - [Publish](#publish)

## Contribute

Choose the language in which you want to write. Then your article may be translated into another language with an indication of the author. Now available in Russian `ru` and English `en`.
Create a file with the name of the path where the page will be accessible, for example new file `/en/tutorials/edge-insets-uibutton`.

### Content

You can set text, pictures and video. I offer my hosting, but you can use any other. Try not to use large videos - users don't like long loading times. If you want use my hosting, simple send me archive with files and path of article - I will add shortly.

### Formatting

Basic markdown functions are supported, like title, subtitle and paragraph. Also available link, images and video. Here provided list:

```
// Titles
# Title
## Subtitle
### Paragraph

// Link
[Link Name](url)

// Formatting
***bold***
>Text that is a quote

// Image and video
![Image Description](https://myoctocat.com/assets/images/base-octocat.svg)
[Video Description](https://cdn.ivanvorobei.by/websites/sparrowcode.io/drag-and-drop-part-1/drag-delegate.mov)
```

For higlight link to grey area with title and subtitle, use this custom formatting:
```
[title](url): description
```
Example [here](https://sparrowcode.io/resources-for-ios-developer).

### Meta

Fill in the details of the article for file [/en/meta/articles.json](/en/meta/articles.json). If the article already exists, set the date of the last change and indicate yourself as editor or translator. All fields are listed here, some of them are optional.

- `title` - Title of your tutorial.
- `description` - Description of tutorial.
- `category` - Category ID, read next section.
- `author` - Author ID, read next section.
- `keywords` - Array of relative keys for your article.
- `updated_date` - Date of last updating article. Format `01.01.2022`.
- `added_date` - Date of created article. Format `01.01.2022`.

##### Optional

- `editors` - Array of author IDs. If you fix some typos, add username here. 
- `translator` - Author ID.

List of categories available at [/en/meta/categories.json](/en/meta/categories.json). If you need an additional category, add it. Make sure none of the existing ones fit.

Authors available at [/en/meta/authors.json](/en/meta/authors.json). Fill in a short information about yourself, you can add buttons to the GitHub or your page in the App Store.

### Publish

Push changes and make pull request. I will approve it shortly and it will be available on website.
