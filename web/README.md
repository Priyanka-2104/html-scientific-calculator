# Web Calculator

This is a simple client-side calculator that supports arithmetic and trigonometric expressions.

Features:
- Evaluate arithmetic expressions, powers, parentheses, factorials, logs, etc.
- Trigonometric functions: `sin`, `cos`, `tan`, `asin`, `acos`, `atan`.
- Angle units: toggle between **Radians** and **Degrees** (top-right of the UI).
- Degree-specific helpers: `sin_deg(x)`, `cos_deg(x)`, `tan_deg(x)`.

How to use:

- Open the UI in your browser: open [web/index.html](web/index.html) (file://) or serve the folder with a simple HTTP server.

Run with Python's simple server:

```bash
cd "c:\Users\Admin\Downloads\my project\calculator\web"
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

Security note:
- The app uses math.js for expression parsing and evaluation with a whitelist of functions. It is intended for local use and demos; do not run untrusted user input on a public site without additional sandboxing.
