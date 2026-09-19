# Rescue the Groom — public pages

The support and privacy pages for the **Rescue the Groom** iOS app, served by
GitHub Pages:

- Support: <https://rescuethegroom.com/>
- Privacy policy: <https://rescuethegroom.com/privacy-policy.html>

Both URLs are required fields in App Store Connect.

## Why this is a separate repository

The app itself lives in the private `rescue-the-groom` repo, and it stays
private: it contains all 113 card images, which carry real wedding guests'
names and likenesses. GitHub Pages is not available on private repositories
without a paid plan, and making that repo public to get Pages would publish
exactly the material the app's access gate exists to protect.

So only these two files — which contain no personal data — are public.

## Keeping them in step

The source of truth is `docs/` in the app repo, and the privacy wording is
shared with the in-app copy in `src/ui/privacyText.ts`. Edit there, then copy
the files here. If you change what the app collects, all three change together.
