# Complete Lucas Rabelo website update — install at repository ROOT

Repository: https://github.com/marreapato/marreapato.github.io

## Why the previous updates looked incomplete

GitHub still showed `_data/profile.yml` containing `Your Name`, the cat biography, placeholder school names, and a commented-out LinkedIn field. The four real news entries existed, but six fictional template news items also existed, and sample blog/showcase cards were still published.

## Install all at once

1. Extract the ZIP. It contains `_data`, `_includes`, `_news`, `_posts`, `_showcase`, `_config.yml`, `index.html` and this README.
2. Copy everything **inside** the extracted directory into the ROOT of `marreapato/marreapato.github.io` (`main` branch), **preserving folder paths and overwriting matching files**. Do NOT create a nested `lucas_complete_site_update` folder.
3. Commit and wait for GitHub Pages to redeploy (check the repository's Actions tab).
4. Hard refresh https://marreapato.github.io/ (Ctrl+Shift+R). Check the main name, portrait, LinkedIn icon, About Me, Education, Experience, News & Milestones, Blog, Showcase, and publication page.

### What changed

- `_data/profile.yml` fixes name, affiliation, email, Google Scholar ID, GitHub, LinkedIn, biography, education, positions, volunteering, experience, and honors. Uses existing `assets/images/photos/portrait.jpg` (not included in ZIP; already in repository).
- `_includes/widgets/experience_card.html` skips missing logos to avoid broken icons.
- `_includes/widgets/news_card.html` excludes hidden template entries and labels section News & Milestones.
- `_news/` provides four dated real announcements and overwrites six fictitious template entries with `show: false`.
- `_posts/` provides three original blog posts and de-publishes three template demo posts.
- `_showcase/profile/` adds four visible real cards; existing unrelated demo cards in `_showcase/default/` and `_showcase/cats/` are set to `show: false`.
- Homepage now provides prominent Blog and Showcase links, omits debug widgets, and displays News after education/experience.
- `_config.yml` sets baseurl to empty for the root GitHub Pages site.

### Important

GitHub's browser uploader can be awkward for directory uploads. The safest one-step method is to extract the ZIP into a LOCAL CLONE, then commit/push the resulting changes:

```bash
git clone https://github.com/marreapato/marreapato.github.io.git
cd marreapato.github.io
# Copy extracted contents INTO this folder, overwriting matching files.
git add .
git commit -m "Update Lucas Rabelo profile, news, blog and showcase"
git push origin main
```

This is a file overlay, **not** a full replacement repository. Do not delete your existing `assets`, styles, layouts, or publications. If your local profile contains newer edits than the publicly readable GitHub version, compare those before overwriting.

The titles and articles use information from your LinkedIn profile PDF and the EBDVF experience you described. Research descriptions were informed by your stated PhD interests. Dates and first-person wording should be checked before publication.
