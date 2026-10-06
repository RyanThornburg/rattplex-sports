# Rattplex Sports

A static landing page that links to the sports sites:

- [Petz Pool](https://splash.rattplex.com/) ([splash-sports-standings](https://github.com/RyanThornburg/splash-sports-standings)): the friend group's view of a Splash Sports college football pick'em
- [Morlocked Pick'em](https://morlocked.rattplex.com/) ([cbs-pickem-web](https://github.com/RyanThornburg/cbs-pickem-web)): the CBS NFL pick'em pool dashboard
- [TheeeeOPlex](https://ncaa.rattplex.com/) ([ncaa-tournament-draft](https://github.com/RyanThornburg/ncaa-tournament-draft)): the NCAA tournament team draft

It's one HTML file, `public/index.html`, with no build step.

## Deploy

It's served as a Cloudflare Worker that only has static assets:

```sh
npx wrangler deploy
```

Then add a custom domain (e.g. `sports.rattplex.com`) to the Worker in the Cloudflare dashboard.
