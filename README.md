# fromkoyomi.org

The home page for Koyomi's apps. It is plain HTML and CSS: no build step, no JavaScript, no cookies and no requests to other sites.

- `index.html` and `style.css` are the page.
- `fonts/` holds Darker Grotesque and Space Mono as WOFF2, converted from the files in Kitae for iPhone, with their SIL Open Font License texts.
- `favicon.svg` and `apple-touch-icon.png` are the cairn mark.

The colours are Kitae's own (`Shared/Colors.xcassets` in kitae-ios), apart from the orange heart and Tabe's persimmon, and the page follows the phone's light or dark setting.

## Preview

Serve the folder and open it in a browser:

```bash
python3 -m http.server 8000
```

## Keeping it private

The `Content-Security-Policy` tag in `index.html` only allows files from this site. If you add something that loads from somewhere else (a font service, an analytics script, an embed), the browser will block it. That is on purpose.
