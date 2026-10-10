# GitHub Pages profile update

Repository: https://github.com/marreapato/marreapato.github.io

Changes:
1. `_data/profile.yml` replaces the template placeholder with Lucas Rabelo's biography, education, positions, experience, awards, social links, and the existing portrait.
2. `_config.yml` sets `baseurl: ""` for a GitHub Pages user website hosted at the domain root.
3. `_includes/widgets/experience_card.html` prevents missing school/company logos from rendering as broken images when no `logo` is defined.

The existing photo is already present at `assets/images/photos/portrait.jpg` in the repository. No image needs to be uploaded. The image file is approximately 16.4 MB; optionally compress it separately for faster loading.

To apply: copy these files into the same paths in the GitHub repository on a new branch, then open a pull request to `main`. Review the content and preview the built site before merging.

Note: GitHub connector branch creation was denied (403: Resource not accessible by integration). Nothing was changed on the live repository.
