# Mohammad Sadeghi — academic homepage

A personal academic website based on [Academic Pages](https://github.com/academicpages/academicpages.github.io).

## Publish the initial version

This checkout is connected to `https://github.com/sadeghi1996m/sadeghi1996m.git`, on the `master` branch.

1. Commit and push the changes **inside this repository folder**. In VS Code, open this folder, review Source Control, stage all website changes (including removed template examples), commit, and use **Sync Changes**.
2. Open [the repository's Pages settings](https://github.com/sadeghi1996m/sadeghi1996m/settings/pages).
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select **master** and **/(root)**, then **Save**.
5. Wait for the Pages deployment in the **Actions** tab to finish.
6. Visit **https://sadeghi1996m.github.io/sadeghi1996m/**.

The `Validate website` workflow checks that the website builds. GitHub's separate Pages workflow publishes it after Pages is enabled. No local Ruby installation is required to publish from GitHub.

## Optional: use the shorter homepage address

To publish at `https://sadeghi1996m.github.io/`:

1. Rename the repository to `sadeghi1996m.github.io` in GitHub's **Settings → General**.
2. Change these entries in `_config.yml`:
   ```yaml
   baseurl: ""
   repository: "sadeghi1996m/sadeghi1996m.github.io"
   ```
3. Keep `url: "https://sadeghi1996m.github.io"`.
4. Update the local Git remote to the renamed repository, then commit and push the configuration change.

The current configuration works with the existing repository name; renaming is optional.

## Edit content

| File | Content |
| --- | --- |
| `_config.yml` | Name, photo, contact links, website address |
| `_pages/about.md` | Homepage biography and interests |
| `_pages/research.md` | Research summaries |
| `_data/publications.yml` | Published papers and the submission under review |
| `_pages/teaching.html` | Teaching experience |
| `_data/navigation.yml` | Navigation menu |
| `_sass/layout/_personal.scss` | Personal styling |
| `images/mohammad-sadeghi.png` | Profile photograph |

Publication details and teaching dates follow the supplied CV. Update the submitted letter's status when it changes.

There is no CV page or download. The sibling `CV` and `Research Statement` folders are local reference material and should stay outside this repository. The GitHub profile link is hidden until a username is added to `author.github` in `_config.yml`.

## Local preview (optional)

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Open **http://127.0.0.1:4000/sadeghi1996m/**. Restart Jekyll after changes to `_config.yml`.

## Credits

This website retains the Academic Pages / Minimal Mistakes theme. See `LICENSE`.
