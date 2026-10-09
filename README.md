# Vancouver bike marketplace feed

Curated public Facebook Marketplace bicycle listings around Vancouver, BC, near C$100. The feed is refreshed every six hours.

Machine-readable feed: [bikes.json](bikes.json) ([raw JSON](https://raw.githubusercontent.com/dgootman/vancouver-bike-marketplace-feed/main/bikes.json)).

Each listing includes a Marketplace ID and URL, title, make, model, type, price in CAD, source, estimated posting date, the age displayed by Marketplace, verification time in UTC, full seller posting text, and an image URL. A null make or model means the listing did not identify it clearly. The `date_posted` field is an estimate based on relative age shown by Marketplace; `date_posted_display` preserves that wording and `date_posted_is_estimate` marks the uncertainty.

Listings and prices may change or disappear between checks. `availability` remains unverified until the seller confirms it. Facebook image URLs may expire.
