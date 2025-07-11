# This Is Archify | [Try It Yourself!](https://archify.strangled.net/?callback=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DdQw4w9WgXcQ)
**DISCLAIMER:** Not Sponsored or Endorsed by McDonald's Restauraunts.
## Introduction
Hey, developers! Want a no-frills way to verify where your users are in the United States, without being invasive with their data? 

And users! Tired of having to give your and personal information to almost every website, just to verify your location?

Well, I've created the most American way to verify a user's location in the United States: **Archify.**
## How It Works
Instead of sharing where, exactly, the user is, the user has to pull in within range to a McDonald's restauraunt, then tap the `I'm Here` button.

Yes--your users, literally, has to drive to a McDonald's and tap `I'm Here`.

Once verified, we simply share the city and state of the McDonald's with the developer--no spesific information, no invasive data, just a simple verification.

The entire process happens client-side on their device, so I know nothing, and the developer only knows the city and state of the McDonald's once the user taps `Authorize`.
## Developer Implementation:
The API is free to use by any and all developers!

Our endpoint is: `https://archify.strangled.net/?callback=[YOUR URL]`

**NOTE:** `[YOUR URL]` is the URL-encoded website link you want Archify to redirect your users to after the check. This can contain GET parameters, but none of them can be named `archify`. Please include `https://` or `http://` at the start of the URL--if not, we'll assume `https://`. 

Once your users has tapped `Authorize`, they'll be redirected to `[YOUR URL][? or &, depending on if you have any other GET parameters]archify=[CITY],[STATE]`. 

**NOTE (x2):** If the McDonald's city or state is unknown, the city or state should appear as `UNKNOWN`.
# Credits
- **[viv](https://github.com/vivcod3s/)** - Developer
- **[Donators](https://vivianbostick.com/donate.php)** - Thank You!
- **[Overpass API](https://overpass-api.de)** - Find McDonald's Locations
- **[Github Pages](https://pages.github.com)** - Hosting
- **[FreeDNS](https://freedns.afraid.org)** - Access to the `Archify.strangled.net` subdomain
