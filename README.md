# H. I. Samyuktha — Portfolio Website

A personal portfolio website with 10 pages, built with HTML, CSS, and vanilla JavaScript.

---

## Pages

| Page | File | Purpose |
|------|------|---------|
| Home | `home.html` | Hero, bio, portrait |
| Experience | `experience.html` | Career timeline |
| Expertise | `expertise.html` | Skills & domains |
| Writings | `writings.html` | Articles & essays |
| Achievements | `achievements.html` | Awards & honours |
| Events | `events.html` | Events organised/attended |
| LinkedIn | `linkedin.html` | Backlinked LinkedIn posts |
| Gallery | `gallery.html` | Photo wallet / gallery |
| Diary | `diary.html` | Private journal entries |
| Connect | `connect.html` | Contact & open channels |

---

## How to add content

### Add a portrait photo
1. Save your photo as `assets/photos/portrait.jpg`
2. It will automatically appear on the Home page

### Add gallery photos
1. Save photos to `assets/gallery/`
2. Open `gallery.html`, find the REAL PHOTO TEMPLATE comment
3. Copy the template, set `src="assets/gallery/your-file.jpg"`, fill in captions

### Add LinkedIn posts
1. Go to your LinkedIn post → click ••• → "Copy link to post"
2. Open `linkedin.html`, find the TEMPLATE comment, paste the link in `href=""`
3. Fill in title, excerpt, date, type

### Add articles (Writings page)
1. Open `writings.html`
2. Find the TEMPLATE comment at the bottom of the writing-grid
3. Copy it, set `href="your-article-url"`, update badge to `published`

### Add diary entries
1. Open `diary.html`, find the ADD NEW ENTRIES comment
2. Copy any `.diary-entry` block and fill in date, category, title, body text
3. Set `data-year` and `data-cat` (moral / meeting / learning / experience / reflection)

### Add events
1. Open `events.html`, copy a `.event-card` block
2. Set `data-type="organized"` or `data-type="attended"`

### Add experience roles
1. Open `experience.html`, copy a `.tl-item` block inside the timeline

---

## Deploying to GitHub Pages (step by step)

### First time setup

1. **Create a GitHub account** at github.com if you don't have one

2. **Create a new repository**
   - Click the "+" button → "New repository"
   - Name it: `samyuktha-portfolio` (or any name you like)
   - Set it to **Public**
   - Do NOT check "Add README" (you already have one)
   - Click "Create repository"

3. **Upload your files**
   - On the new repo page, click "uploading an existing file"
   - Drag and drop the entire unzipped portfolio folder contents
   - Click "Commit changes"

4. **Enable GitHub Pages**
   - Go to your repo → Settings → Pages (left sidebar)
   - Under "Source", select: **Deploy from a branch**
   - Branch: `main` → Folder: `/ (root)`
   - Click Save
   - Your site will be live at: `https://yourusername.github.io/samyuktha-portfolio/`

5. **Your live URL** will appear at the top of the Pages settings after ~1 minute

---

## Editing in GitHub Codespaces (for future updates)

Codespaces lets you edit code directly in your browser — no software needed.

1. Go to your repository on github.com
2. Press the `.` key (period) on your keyboard — this opens VS Code in the browser instantly
   - OR click the green "Code" button → "Codespaces" tab → "Create codespace on main"
3. You'll see all your files in the left sidebar
4. Click any HTML file to edit it
5. When done, go to Source Control (the branch icon on the left) → type a commit message → click the ✓ Commit button
6. Your changes go live on GitHub Pages automatically within ~1 minute

### Tip: Preview while editing
In Codespaces, right-click any HTML file → "Open with Live Server" to see changes in real time.

---

## File structure

```
samyuktha-portfolio/
├── index.html          ← redirects to home.html
├── home.html
├── experience.html
├── expertise.html
├── writings.html
├── achievements.html
├── events.html
├── linkedin.html
├── gallery.html
├── diary.html
├── connect.html
├── css/
│   └── main.css        ← all shared styles
├── js/
│   ├── nav.js          ← theme + reveal logic
│   └── nav-inject.js   ← shared nav HTML
└── assets/
    ├── photos/
    │   └── portrait.jpg  ← add your portrait here
    └── gallery/
        └── (add photos here)
```

---

## Customisation tips

- **Email**: Open `connect.html`, find `href="mailto:your@email.com"` and replace with your email
- **Theme**: The site defaults to dark mode. Users can toggle light/dark — their preference is saved
- **New year in diary**: Open `diary.html`, add a `<button>` in `.year-selector` for the new year
- **New achievement category**: Open `achievements.html`, add a new `.ach-tab` and `.ach-panel`
