# Double Eagle Ranch Website

![GitHub
Pages](https://img.shields.io/github/deployments/doube-eagle/website/github-pages?label=pages&logo=github)

A simple solution for our current neighborhood website.

## Update Members

Edit `site-data.json` to add new board or committee members. Follow the convention in the file, it's
json it can be pasted into a [json validator](https://jsonlint.com) to verify the format is correct.

Changing the number of members will work too (for example, increasing the board from 3 to 5).

It doesn't allow adding new committees yet.

## Development

- Web browser: open `index.html`
  - Note: won't show data defined in `site-data.json`, but works for making other changes
  - The `site-data.json` can temporarily be copied to `index.html` inside a `<script>` tag
- Docker: `docker run -d -p 8080:80 --rm -v $(pwd):/usr/share/nginx/html nginx`
- Any web sever, [python](https://stackoverflow.com/a/27986564) or
  [node](https://stackoverflow.com/a/23122981), works too
