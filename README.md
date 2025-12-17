# TSOSI's newsletter

This repo contains the content of the newsletter that was sent

the newsletter is done with [maily.to](https://maily.to/)

## Add a newsletter

To add a newsletter, just drop the **html file** in this repo.  
Files should be named by their date of publication in iso format (`YYYY-MM-DD.html`).  
Date of month (`-DD`) is optional but could be useful if we publish more that one newsletter in a month.

```
- 2025-10.html
- 2025-08-12.html
- 2025-08.html
- 2024-12.html
```

## Technical

[TSOSI's app](https://github.com/tsosi-org/tsosi-app) uses this repository to generate [tsosi.org/pages/newsletter](https://tsosi.org/pages/newsletter)   

Specific newsletter will be served on dedicated urls based on filenames
 [tsosi.org/pages/newsletter/2025-10](https://tsosi.org/pages/newsletter/2025-10) -> `2025-10.html`

Files are listed with github API : [api.github.com/repos/tsosi-org/newsletter/contents](https://api.github.com/repos/tsosi-org/newsletter/contents)

**Newsletter's name** is automatically generated based on the publication date in the file name  
`2025-10.html` -> `Newsletter October 2025`

**Newsletter's keypoints** are extracted from the html content using `h2`,`h3` html tags. (Corresponding to `##` and `###` entries in maily's markdown).
