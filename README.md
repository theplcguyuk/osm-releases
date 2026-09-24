# OSM firmware releases

Signed firmware and web UI images for the Tryac Off Site Monitor (OSM1, OSM1+, OSM2).
Source code is kept in a separate private repository.

OSM devices download updates from this repo's GitHub Pages site:

    https://theplcguyuk.github.io/osm-releases/ota/<OSM1|OSM1Plus|OSM2>/index.json

Every image is Ed25519-signed; devices reject anything not signed with the Tryac
key, built for a different product, or older than the installed version.

Files under `ota/` are published by `shared/tools/publish_ota_pages.py`
(normally via `build-ota.ps1`) — do not edit them by hand.
