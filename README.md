# Buddy — Eats the World test copy

An isolated static copy for testing `buddy.eats-the-world.com`. The original [Buddy project](https://github.com/tjansn/Buddy) and its existing Pages site remain unchanged.

`index.html`, `assets/buddy-screen-renderer.js` and the MIT `LICENSE` are copied byte for byte from Buddy commit [`42076a0b149d685dc2fa993a7c1ee22d6a015d6a`](https://github.com/tjansn/Buddy/tree/42076a0b149d685dc2fa993a7c1ee22d6a015d6a). Existing copyright notices, source links and attribution are retained. No firmware, device tools or source history are included.

Recommended repository: `tjansn/buddy-etw-test`. The `main` workflow publishes only the static page, renderer, license, `.nojekyll`, and an optional verification file. There are no API credentials or backend services in this repository.

For the DNS test, add `.well-known/eats-the-world` containing the **current token issued for the real `buddy` claim** after its CNAME destination is saved as `tjansn.github.io`. No placeholder is provided or published. The build rejects malformed proof contents. A token's shape alone does not prove its validity: Eats the World must still check the exact token against the current claim and server response.

Configure only this test repository's Pages custom domain as `buddy.eats-the-world.com`. GitHub Pages must serve the proof directly over HTTP with status 200 before Eats the World publishes the DNS record; coordinate HTTPS enforcement and certificate provisioning with that check. Never bypass verification or change the original `tjansn/Buddy` repository's Pages settings.

The test approval is time limited. Coordinate renewal or removal of the DNS and custom-domain setting before it expires. The original Buddy URL remains independent of this test copy.
