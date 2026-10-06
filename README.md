# Mohammad Sadeghi — academic homepage

A personal academic website based on [Academic Pages](https://github.com/academicpages/academicpages.github.io).

## Publish at the root homepage address

The publishing branch is **Deploy**. The configuration now targets **https://sadeghi1996m.github.io/**.

1. On GitHub, open the existing repository's **Settings → General** and rename it from `sadeghi1996m` to **`sadeghi1996m.github.io`**. The local folder can keep its current name.
2. In a terminal inside this repository, update the local remote:
   ```sh
   git remote set-url origin https://github.com/sadeghi1996m/sadeghi1996m.github.io.git
   ```
3. Commit and push the prepared changes on **Deploy**. In VS Code, review Source Control, stage the changes, commit, and use **Sync Changes**.
4. Open [the renamed repository's Pages settings](https://github.com/sadeghi1996m/sadeghi1996m.github.io/settings/pages). Under **Build and deployment**, select **Deploy from a branch → Deploy → /(root)**, then **Save** if needed.
5. Wait for **pages build and deployment** in the **Actions** tab to finish successfully.
6. Visit **https://sadeghi1996m.github.io/**. If an older page appears, refresh with **Ctrl+F5**.

The `Validate website` workflow checks pushes to `Deploy`, `master`, and `main`. GitHub's separate **pages build and deployment** workflow publishes the branch selected in Pages settings. No local Ruby installation is required to publish from GitHub.

## Why the old address included the repository name

GitHub treats `sadeghi1996m/sadeghi1996m` as a project site, so its address is `https://sadeghi1996m.github.io/sadeghi1996m/`. Naming the repository `sadeghi1996m.github.io` makes it the account's root homepage. The branch name does not determine the public URL.

If you decide to retain the original repository name, restore `baseurl: "/sadeghi1996m"` and `repository: "sadeghi1996m/sadeghi1996m"` in `_config.yml` before publishing.

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

Open **http://127.0.0.1:4000/**. Restart Jekyll after changes to `_config.yml`.

## Credits

This website adapts [Academic Pages](https://github.com/academicpages/academicpages.github.io), originally forked by Stuart Geiger from [Minimal Mistakes](https://mademistakes.com/work/jekyll-themes/minimal-mistakes/) by Michael Rose. Academic Pages is maintained by Robert Zupko and contributors. The site is generated with [Jekyll](https://jekyllrb.com).

The original [MIT license](LICENSE), including `Copyright (c) 2016 Michael Rose`, is retained unchanged. MIT permits modification and redistribution provided its copyright and permission notices remain with copies or substantial portions of the software. Keep this file and the notices belonging to bundled third-party components when redistributing the site code.

The published site includes the full theme license at `/LICENSE`, linked from the footer. The visible theme credits acknowledge the source projects; the MIT license does not specifically require a footer link. The footer's personal copyright line refers to site content, not ownership of the upstream theme.
