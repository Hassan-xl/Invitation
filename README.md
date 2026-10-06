# Warisha & Abdul Wassay · Wedding Invitation

A static website. No build step, no dependencies.

| File | What it is |
|---|---|
| `index.html` | The invitation itself (sealed letter, story, dates, countdown) |
| `couple.jpg` | The couple's photo shown in the arch |
| `og.jpg` | The preview image WhatsApp and Facebook show when the link is shared |
| `favicon.png` | Wax-seal icon for the browser tab |
| `apple-touch-icon.png` | Icon when a guest adds the page to their phone's home screen |

## Put it online (GitHub + Vercel)

1. Create a new GitHub repository and upload all the files in this folder to the root of the repository.
2. In Vercel, choose **Add New → Project**, then import that repository.
3. Set **Framework Preset** to **Other**. Leave the build command empty and keep the output directory as the root.
4. Press **Deploy**. Every later push to GitHub updates the live site automatically.

## Two things to check before sending to guests

**1. Your live address.** The link-preview tags in `index.html` point to
`https://warisha-abdulwassay.vercel.app`. If your Vercel address or custom domain is different,
search `index.html` for `warisha-abdulwassay.vercel.app` and replace all of them with your real address.
WhatsApp only shows the preview image when this address is correct.

**2. The venue map.** Search `index.html` for `MAP_URL` and replace the search link with the exact
Google Maps link for Emerald Banquet (in Google Maps: Share → Copy link).

## Personal links for each guest

Add the guest's name to the end of the link. The envelope will say "Specially for …" and the
letter will open with "Dear …,".

- `https://your-address/?to=Ahmed Family`
- `https://your-address/#Ahmed-Family`

## Good to know

- WhatsApp remembers a link's preview. If you shared the link before the preview was right,
  test with a fresh variant such as `?to=Test` to see the updated card.
- The countdown and calendar buttons use the times in the `EVENTS` block of `index.html`
  (written in UTC: 4:00 pm in Pakistan is 11:00 UTC, 10:00 pm is 17:00 UTC).
- The background music is generated live by the page itself, so there is no audio file to host.
  Guests can pause it with the gold button at the bottom right.
