# Carrot Locks Records
**Pretoria's Independent Amapiano Label · carrotlocks.co.za**

Pure HTML & CSS — hosted on GitHub Pages. No JavaScript. No server required.

---

## Files

```
carrotlocks-github/
├── index.html      ← The entire website
├── css/
│   └── style.css   ← All styling
└── assets/
    └── img/        ← Drop artist photos + cover art here
```

---

## How to host on GitHub Pages (free)

1. Create a free account at **github.com**
2. Click **New repository** → name it `carrotlocks.co.za` or `carrotlocks-site`
3. Upload `index.html`, `css/style.css`, and your `assets/` folder
4. Go to **Settings → Pages → Source → main branch → / (root)**
5. GitHub gives you a free URL like `yourname.github.io/carrotlocks-site`
6. To use your own domain (`carrotlocks.co.za`): add it under **Settings → Pages → Custom domain** and set a CNAME record in your domain DNS pointing to `yourname.github.io`

---

## What to update (all marked with ✏️ in the HTML)

### Coming soon banner
Find the `COMING SOON BANNER` section and update the release title and artist name.

### Releases
Find each `.release-card` and update:
- The `href` link (Apple Music URL for that release)
- The title, artist name, and meta text
- To add artwork: place image in `assets/img/` and add `<img src="assets/img/cover.jpg" alt="Title">` inside the `.release-card__art` div

### Artists
Find each `<article class="artist-card">` and update:
- The gradient colours (optional)
- Artist name, genre, release count
- Latest release name
- Apple Music link
- To add a photo: add `<img src="assets/img/artist.jpg" alt="Name">` inside `.artist-card__art`

### The Vault (Exclusive Store)
1. Sign up at **gumroad.com** (free)
2. Create a product for each track → upload your audio files
3. Copy the product URL from Gumroad
4. Replace each `href="https://carrotlocks.gumroad.com/l/..."` with your real links
5. Update price, title, artist, and description

### Booking Form
1. Sign up at **formspree.io** (free — 50 submissions/month)
2. Create a new form → copy the form ID (e.g. `xpwzgkqr`)
3. In `index.html`, find `YOUR_FORMSPREE_ID` and replace it
4. Submissions go straight to your email

### Newsletter
**Option A (simple):** The default `mailto:` form already works — clicking Subscribe opens the user's email app.

**Option B (proper):** Sign up at **mailchimp.com** (free up to 500 contacts) → Audience → Signup forms → Embedded forms → copy the `<form>` HTML and replace the newsletter form in `index.html`.

### Social & streaming links
Search for `href="#"` in the footer and nav and replace with your real links.

---

## Adding a new release
1. Open `index.html`
2. Find the releases section
3. Copy one complete `<a class="release-card">` block
4. Paste it at the top of the grid
5. Update the link, title, artist, and art colour class (`art--a` through `art--f`)

## Adding a new Vault product
1. Open `index.html`
2. Find the vault section
3. Copy one `<div class="vault-card">` block
4. Paste it into the grid
5. Update title, artist, price, description, and Gumroad link
