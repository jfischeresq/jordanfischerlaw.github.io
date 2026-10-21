# Fischer Law, P.C. website

Jekyll site hosted on GitHub Pages at jordanfischerlaw.com.

- Page content lives in the `.md` files at the root (`aboutus.md`, `ourservices.md`, etc.).
- Attorney bios live in `_team/`. Add `role`, `order`, `credentials`, and `image_path` in the front matter.
- Insights posts live in `_posts/` as `YYYY-MM-DD-title.md`. Add a one-sentence `description` and optional `image` in the front matter.
- Shared contact details (email, phone, LinkedIn) are set once in `_config.yml`.
- All styling is in `style.scss`. The site uses system fonts and inline icons, so it makes no third-party requests.
