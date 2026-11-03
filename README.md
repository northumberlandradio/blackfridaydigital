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

The form sends to **tommyw@mbcmedia.ca** through [Web3Forms](https://web3forms.com), a free form service for static sites.

1. Go to https://web3forms.com, enter **tommyw@mbcmedia.ca** and click **Create Access Key**.
2. Web3Forms emails the key to that address. Copy it.
3. In `index.html`, find `YOUR_ACCESS_KEY_HERE` and replace it with the key. Commit the change.
4. Submit the form once yourself to test it. You'll land on the thank-you page and the request will arrive in the inbox.

The access key is safe to have in a public page. It can only send email to the address it was created for.

## The video

The video is embedded from YouTube (`TKSicuEyJA8`) with captions turned on by default. To use a different video, search `index.html` for `TKSicuEyJA8` and replace it with the new video's ID.

## Once the spot is booked

In `index.html`, change `1 of 1 left` to `SOLD`, and change the button text if you want to stop taking inquiries.
