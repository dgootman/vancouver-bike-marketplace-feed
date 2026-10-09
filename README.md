# Vancouver bike marketplace feed

Public Facebook Marketplace bicycle listings around Vancouver, BC, up to C$200. The feed is checked every six hours and holds up to 100 listings. Newer listings come first; road bikes come before other types among listings with similar posting dates.

Machine-readable feed: [bikes.yaml](bikes.yaml) ([raw YAML](https://raw.githubusercontent.com/dgootman/vancouver-bike-marketplace-feed/main/bikes.yaml)).

Each listing includes the Marketplace ID and URL, title, make, model, bike type, CAD price, source, posting date, verification time in UTC, full seller posting text, condition, and an image URL when available. A null make, model, type, posting date, or image URL means it could not be established from the visible listing.

Marketplace often shows only a relative posting age. `date_posted` is an estimate in those cases, `date_posted_display` keeps the wording shown, and `date_posted_is_estimate` marks the estimate. Prices and descriptions can change or disappear between checks; seller availability and bike condition still need confirmation. Facebook image URLs may expire.
