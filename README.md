# Parichart — Software Tester Portfolio (Static, for GitHub Pages)

Plain HTML/CSS site — no server needed, so it can be hosted for free on
GitHub Pages and opened by anyone with a link, no localhost required.

## 1. Set up the contact form (Formspree — free)

The site currently has no backend, so the form needs a place to send
submissions to. [Formspree](https://formspree.io) is free for basic use
and works with a static site.

1. Go to https://formspree.io and sign up (free plan is enough).
2. Create a new form → it gives you a URL like
   `https://formspree.io/f/abcdWXYZ`.
3. Open `index.html`, find this line:
   ```html
   <form id="contact-form" class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
   Replace `YOUR_FORM_ID` with your real ID.
4. Save. Submissions will now arrive in your Formspree inbox (and forward
   to your email).

If you skip this step, the form will show an error message when someone
tries to submit it — everything else on the page still works fine.

## 2. Push to GitHub

```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```
(Create the empty repo on github.com first if you haven't.)

## 3. Turn on GitHub Pages

1. On your repo page: **Settings → Pages**.
2. Under "Build and deployment" → Source: **Deploy from a branch**.
3. Branch: **main**, folder: **/(root)** → **Save**.
4. Wait ~1 minute, then refresh — GitHub shows the live URL, usually:
   ```
   https://YOUR_USERNAME.github.io/YOUR_REPO/
   ```

That link works for anyone, on any device — no localhost, no PHP, no
server setup needed on their end.

## Editing content later

All the text (name, about, testing toolbox, projects) lives directly in
`index.html`. Since this is a static export (no more PHP arrays), edit
the HTML directly — search for the section you want (`id="about"`,
`id="skills"`, `id="project"`, `id="contact"`) and change the text
in place.

## Files
```
index.html      Full page
style.css        All styling
images/          Photos and project screenshots
```
