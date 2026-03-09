# ModernStream Blog 📊

> **Niche:** Storytelling with Data  
> **Stack:** Pure HTML + CSS + Vanilla JavaScript (Zero dependencies)  
> **Deploy:** GitHub Pages / Hostinger

---

## 🚀 Features

- ✅ Light / Dark mode (localStorage persistent, smooth 0.3s transition)
- ✅ SPA hash-based router (Home, Archive, Single Post, Category, About, Contact, 404)
- ✅ Sticky header with scroll shadow
- ✅ Search overlay (live filtering)
- ✅ Featured posts section + grid layout
- ✅ Sidebar: Search, Recent Posts, Categories, Newsletter
- ✅ Single post: Author box, Share buttons, Related posts, Comments
- ✅ Reading progress bar
- ✅ Scroll reveal animations (IntersectionObserver)
- ✅ Back to top button
- ✅ Responsive: Desktop / Tablet / Mobile
- ✅ SEO-friendly HTML structure
- ✅ Zero npm / Zero build step

---

## 📁 File Structure

```
modernstream-blog/
├── index.html          ← Shell + Header + Footer
├── style.css           ← All styles (CSS variables, dark mode, responsive)
├── README.md
└── js/
    ├── data.js         ← Blog posts & categories data
    └── app.js          ← Router + all page renderers
```

---

## 🌐 Deploy to GitHub Pages

```bash
# 1. Create a repo on github.com
git init
git add .
git commit -m "Initial commit — ModernStream Blog"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/modernstream-blog.git
git push -u origin main

# 2. Go to repo → Settings → Pages → Source: main / root → Save
# Your site is live at: https://YOUR_USERNAME.github.io/modernstream-blog/
```

---

## 🟠 Deploy to Hostinger

1. Log in to Hostinger → **Hosting** → your plan → **Git**
2. Click **Connect with GitHub** → authorize
3. Select the `modernstream-blog` repo → branch `main`
4. Set root folder to `/` → **Deploy**
5. Every `git push` auto-deploys ✅

Or manually: zip the folder → **File Manager** → upload to `public_html/`

---

## ✏️ Add Content

Edit `js/data.js` — add a new object to the `POSTS` array:

```js
{
  id: 10,
  slug: "my-new-article",
  title: "My New Article Title",
  excerpt: "Short description shown in cards.",
  category: "Data Viz",
  cat_slug: "data-viz",
  date: "March 10, 2026",
  read_time: "5 min",
  featured: false,
  color: "#5b6cff,#00d4ff",
  emoji: "📈"
}
```

To add full article body, edit the `renderPost()` function in `js/app.js`.

---

## 🎨 Customize Colors

In `style.css`, edit the `:root` block:

```css
:root {
  --primary: #5b6cff;
  --secondary: #ff4d6d;
  --accent: #00d4ff;
}
```

---

## 📝 License

MIT — free to use, modify, and deploy.
