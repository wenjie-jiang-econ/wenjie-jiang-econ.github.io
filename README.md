# Wenjie Jiang Academic Website

This is a simple personal academic website for Wenjie Jiang. It is a static website, which means it is made from ordinary HTML, CSS, JavaScript, images, and PDF files. You do not need a build system to preview or publish it.

## Preview the Website Locally

The easiest way is to open `index.html` in your browser.

You can also run a small local web server from this folder:

```powershell
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Where to Edit Each Section

Most content is in `index.html`.

- Homepage introduction: search for `id="Home"`
- About: search for `id="About"`
- Research: search for `id="Research"`
- Publications and Working Papers: search for `id="Publications"`
- Teaching: search for `id="Teaching"`
- Academic Activities: search for `id="Activities"`
- CV: search for `id="CV"`
- Contact: search for `id="Contact"`
- Navigation menu: search for `id="mainNav"`
- Page title and search/social preview text: edit the top part inside `<head>`

The main custom style rules are in `css/custom.css`. The file `css/styles_navbar.css` contains Bootstrap layout styles and is usually best left alone.

## Replace the Profile Photo

The current profile image is a neutral placeholder:

```text
images/profile-placeholder.svg
```

To use your own photo:

1. Add your image to the `images` folder.
2. Update the `src` value in `index.html`.
3. Update the `alt` text so it describes the image, for example: `Portrait of Wenjie Jiang`.

## Replace the CV

The website currently shows a clear CV placeholder. When your CV is ready, add it here:

```text
files/Wenjie_Jiang_CV.pdf
```

The `files` folder already exists. After adding your CV PDF, update the CV section and the CV links in `index.html`.

## Add a Publication or Working Paper

In `index.html`, go to the section with:

```html
<section id="Publications">
```

Copy the placeholder paper block and replace:

- the title;
- coauthors;
- status or journal information;
- abstract;
- PDF link or published version link, if available.

Do not list papers that are not ready to be public. Use clear placeholders for items you still need to add.

## Deploy Through GitHub Pages

1. Use the GitHub repository `WenjieJiang99/wenjiejiang.github.io`.
2. Upload or push these website files to that repository.
3. On GitHub, open the repository settings.
4. Go to **Pages**.
5. Choose the main branch and the root folder.
6. Save the settings.
7. Your site should appear at:

```text
https://wenjiejiang99.github.io/wenjiejiang.github.io/
```

After deployment, update the placeholder URL in `index.html` and `sitemap.xml`.

## Connect a Custom Domain Later

If you buy a domain such as `wenjiejiang.com`, you can connect it later.

1. In the GitHub Pages settings, enter your custom domain.
2. GitHub will create or ask you to create a `CNAME` file.
3. In your domain provider's DNS settings, add the records GitHub recommends.
4. After the domain works, update the canonical URL, social preview URL, and sitemap URL.

GitHub's official Pages documentation has the most up-to-date domain instructions.

## Information Still To Add

- Profile photo
- CV PDF
- Email address
- Google Scholar link
- LinkedIn or personal profile links
- Research project descriptions
- Publications and working papers
- Teaching experience
- Academic activities
- Final GitHub Pages URL or custom domain
