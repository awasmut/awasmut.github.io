# devlog

Jekyll + GitHub Pages. Push a post, the site rebuilds in about a minute at
<https://awasmut.github.io>. Editing files from the GitHub web UI works fine.

## Adding a post

1. Put a file in `_posts/` named `YYYY-MM-DD-my-title.md`
   (the title becomes the URL: `/posts/my-title/`).
2. Start it with this front matter, then write markdown:

        ---
        layout: post
        title: My Title
        date: 2026-10-31 09:00
        hero: /assets/img/cover.png     # optional full-width image on top
        hero_alt: what the image is     # optional caption/alt text
        ---

        Your post text. Images and videos inline anywhere.

3. Commit and push. Done.

## Images, video, code

Put files in the repo (they are committed like any other file):

    assets/img/     images (png, jpg, svg)
    assets/video/   short clips (mp4, webm)

Images (markdown, use root-relative paths):

    ![caption](/assets/img/cover.png)

Video, self-hosted, no YouTube:

    <video controls preload="metadata" poster="/assets/img/cover.png">
      <source src="/assets/video/clip.mp4" type="video/mp4">
    </video>

Keep clips short and compressed (a few seconds, 1080p mp4 is fine); very big
repos slow down the Pages build.

Code fences highlight automatically:

    ```c
    int main(void) { return 0; }
    ```

## Cheat sheet for the impatient

    _posts/2026-10-31-some-name.md   ->  /posts/some-name/
    assets/img/x.png                 ->  /assets/img/x.png
    assets/video/x.mp4               ->  /assets/video/x.mp4

Folders and files starting with `_` (except `_posts`, `_layouts`) are ignored
by Jekyll — that is why `assets/` has no underscore.

Optional local preview (needs Ruby+Gem install): `bundle exec jekyll serve`.
