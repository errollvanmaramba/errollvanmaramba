 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index 156003f93e43343469c73e575277085b94586e0a..a2fcdd586be7c8fb56585119557a35fb2a2b078c 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,17 @@
-# errollvanmaramba
\ No newline at end of file
+# errollvanmaramba
+
+Static multi-page website for GitHub Pages with a homepage plus four inner pages.
+
+## Pages
+- `index.html`
+- `pages/about.html`
+- `pages/services.html`
+- `pages/work.html`
+- `pages/contact.html`
+
+## Local preview
+Open `index.html` directly in your browser or serve the repository with a static file server, for example:
+
+```bash
+python3 -m http.server 8000
+```
 
EOF
)
