# DataFlow Pro v3.0 - Product Documentation Presentation

A comprehensive Marp-based product documentation presentation for DataFlow Pro, designed for technical writers and maintainable in version control.

## 📧 Contact

**24f2001777@ds.study.iitm.ac.in**

## ✨ Features

This Marp presentation includes all required elements:

- ✅ **Custom Theme Specification** - Complete custom styling in YAML frontmatter
- ✅ **Page Numbers** - Enabled via `paginate: true`
- ✅ **Background Image** - Cloud infrastructure slide with Unsplash image
- ✅ **Custom Marp Directives** - Multiple directives used throughout:
  - `<!-- _class: lead -->` for title slides
  - `<!-- _backgroundColor: -->` for custom backgrounds
  - `<!-- _color: -->` for text colors
  - `<!-- _paginate: false -->` to hide page numbers on specific slides
  - `<!-- _backgroundImage: -->` for background images
  - `<!-- _header: -->` and `footer:` for headers/footers
- ✅ **Mathematical Equations** - LaTeX formulas for algorithmic complexity:
  - Big O notation: $O(n \log n)$
  - Performance analysis formulas
  - Amdahl's Law
  - Cache optimization equations
- ✅ **Email Address** - Displayed in header, footer, and multiple slides

## 📊 Presentation Content (32 Slides)

1. Title slide with contact information
2. Table of contents
3. Introduction to DataFlow Pro
4. System architecture with columns layout
5. **Cloud-native architecture with background image**
6. Installation guide with code blocks
7. Configuration table
8. API reference with HTTP examples
9. Response format (JSON)
10. Performance analysis with time complexity
11. Advanced performance metrics with multiple equations
12. Best practices (success callout)
13. Common pitfalls (warning callout)
14. Advanced configuration (Python)
15. Security considerations (JavaScript)
16. Monitoring metrics table
17. Performance optimization with SQL
18. Data flow patterns (TypeScript)
19. Testing strategy (Python unittest)
20. Troubleshooting guide
21. Debugging techniques
22. Additional resources
23. Training & certification
24. Roadmap & future features
25. Contributing guide
26. Thank you slide
27. Appendix: Mathematical formulas
28. License information
29. Final contact slide

## 🎨 Custom Theme Features

The presentation uses extensive custom CSS styling:

- Custom color scheme (blue-themed)
- Styled code blocks with syntax highlighting
- Grid layouts for columns
- Custom badges and callout boxes
- Styled tables with headers
- Blockquote styling
- Warning and success boxes

## 📐 Mathematical Formulas Included

1. **Time Complexity:** $T(n) = O(n \log n)$
2. **Query Processing:** $Q(n, m) = O(n \cdot m \cdot \log m)$
3. **Space Complexity:** $M(n, k) = O(n) + O(k \cdot \log n)$
4. **Parallel Processing Speedup:** $S(p) = \frac{T_{\text{serial}}}{T_{\text{parallel}}}$
5. **Cache Hit Rate:** $\text{Hit Rate} = 1 - \frac{1}{1 + \lambda \cdot C}$
6. **Big O Comparison:** $O(1) < O(\log n) < O(n) < O(n \log n) < O(n^2)$
7. **Amdahl's Law:** $S_{\text{max}} = \frac{1}{(1-P) + \frac{P}{N}}$

## 🚀 Usage

### View in VS Code

1. Install the [Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode) extension
2. Open `slides.md`
3. Click the Marp preview button or press `Ctrl/Cmd + Shift + V`

### Convert to PDF/HTML/PPTX

```bash
# Install Marp CLI
npm install -g @marp-team/marp-cli

# Convert to PDF
marp slides.md --pdf

# Convert to HTML
marp slides.md --html

# Convert to PowerPoint
marp slides.md --pptx

# Watch mode for live preview
marp -w slides.md
```

### Serve as HTML Presentation

```bash
# Serve with live reload
marp -s slides.md

# Then open http://localhost:8080 in your browser
```

## 📤 Deploying to GitHub

### Step 1: Create GitHub Repository

```bash
cd "/Users/prachetas/Desktop/Programming/TDS Week 8"

# Initialize git (if not already done)
git init

# Add files
git add slides.md README.md

# Commit
git commit -m "Add Marp product documentation presentation"

# Create repository on GitHub, then:
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

### Step 2: Get Raw GitHub URL

Once pushed, your raw GitHub URL will be:

```
https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO_NAME/main/slides.md
```

**Example:**

```
https://raw.githubusercontent.com/prachetas/dataflow-docs/main/slides.md
```

You can view this URL directly or use it with Marp viewers.

## 🌐 Viewing Options

### Option 1: GitHub with Marp Plugin

Install a browser extension like "Marp Viewer" to view the presentation directly from GitHub.

### Option 2: Deploy HTML Version to GitHub Pages

```bash
# Generate HTML
marp slides.md -o index.html --html

# Push to GitHub Pages branch
git checkout -b gh-pages
git add index.html
git commit -m "Deploy HTML presentation"
git push origin gh-pages

# Enable GitHub Pages in repository settings
# Your presentation will be at: https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

### Option 3: Use Marp CLI Viewer

```bash
# Install and serve
npm install -g @marp-team/marp-cli
marp -s slides.md
```

## 📋 Marp Directives Used

- `marp: true` - Enable Marp processing
- `theme: custom-docs` - Custom theme name
- `paginate: true` - Show page numbers
- `header:` - Global header content
- `footer:` - Global footer content (includes email)
- `style: |` - Inline CSS styling
- `<!-- _class: lead -->` - Center content on slide
- `<!-- _paginate: false -->` - Hide page numbers
- `<!-- _backgroundColor: #color -->` - Custom background color
- `<!-- _color: #color -->` - Custom text color
- `<!-- _backgroundImage: url() -->` - Background image
- `<!-- _header: '' -->` - Override header on specific slide

## 🎯 Version Control Benefits

- **Plain Text Format** - Easy to diff and merge
- **Git-Friendly** - Track changes line-by-line
- **Collaborative** - Multiple contributors can work simultaneously
- **Portable** - No proprietary formats
- **CI/CD Ready** - Can automate PDF generation in pipelines

## 📦 File Structure

```
.
├── slides.md           # Main Marp presentation
├── README.md          # This documentation
└── index.html         # (Optional) Generated HTML output
```

## 🔗 Quick Links

- [Marp Documentation](https://marpit.marp.app/)
- [Marp CLI](https://github.com/marp-team/marp-cli)
- [Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)
- [Markdown Guide](https://www.markdownguide.org/)

## 📝 Example Raw URL Format

After pushing to GitHub, your raw URL will follow this pattern:

```
https://raw.githubusercontent.com/[YOUR_USERNAME]/[REPO_NAME]/main/slides.md
```

**Replace:**

- `[YOUR_USERNAME]` - Your GitHub username
- `[REPO_NAME]` - Your repository name (e.g., `dataflow-docs`, `product-documentation`, etc.)

---

**Created by:** Technical Writer  
**Email:** 24f2001777@ds.study.iitm.ac.in  
**Date:** December 7, 2025  
**Version:** 3.0.0
