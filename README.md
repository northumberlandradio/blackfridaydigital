# Black Friday Ad Package landing page

A one-page sales site for the MBC Media Black Friday digital display package: $378 (regular $500), only one available, running November 23–30, 2026 on northumberlanddaily.ca and classicrock1079.ca.

It's plain HTML with no build step, so it works on GitHub Pages as-is.

## Files

| File | What it is |
|---|---|
| `index.html` | The landing page |
| `thanks.html` | Shown after someone submits the booking form |
| `images/` | myFM, Classic Rock 107.9 and Northumberland Daily logos, plus the link-preview image |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Put it online with GitHub Pages

1. Create a new repository on GitHub (for example `black-friday`) and make it **Public**.
2. Click **Add file → Upload files** and drag in everything from this folder, including the `images` folder. Commit.
3. Go to **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**. Save.
4. After a minute or two the page is live at `https://<your-username>.github.io/<repo-name>/`.

`.nojekyll` starts with a dot, so some computers hide it. If it doesn't upload, the site still works without it.

## Turn on the booking form (one-time step)

The form sends to **tommyw@mbcmedia.ca** through [FormSubmit](https://formsubmit.co), a free service for static sites.

1. Once the page is live, fill out the form yourself as a test.
2. FormSubmit emails tommyw@mbcmedia.ca an **activation link**. Click it.
3. From then on, every submission arrives in that inbox as a table with the business name, contact name, email, phone, website and what they want to promote. The subject line includes the business name.

Submissions sent before activation are not delivered, so do this test before you share the link.

## The video

The video is embedded from YouTube (`TKSicuEyJA8`) with captions turned on by default. To use a different video, search `index.html` for `TKSicuEyJA8` and replace it with the new video's ID.

## Once the spot is booked

In `index.html`, change `1 of 1 left` to `SOLD`, and change the button text if you want to stop taking inquiries.
