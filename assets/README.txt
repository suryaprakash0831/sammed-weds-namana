Active media files:
- ../images/portrait.webp : image shown near the bottom of the invitation (currently the Jain emblem
  inside an arch). To show a couple photo instead, replace it with a 1024 x 1536 portrait image
  using the SAME filename.
- ../media/bgm.mp3 : wedding background music (loops).
- ../images/share-card.jpg : 1200 x 630 social preview used by WhatsApp and social apps.
- ../images/jain-emblem.webp : the Jain emblem (opening, loader, footer).
- ../images/gopuram*.webp : the white-marble Jain temple used in the opening scroll animation.

Keep these filenames unchanged when replacing media so the page does not make a
failed request before loading a fallback.

BEFORE GOING LIVE: index.html uses https://YOUR-DOMAIN.com/ in the canonical, og:url and og:image
tags. Replace it with your real address, otherwise WhatsApp link previews will not show the card.

Security note: index.html allows its inline JavaScript through a SHA-256 value in
the Content-Security-Policy meta tag. After editing anything inside the <script>
block, recalculate that hash and update script-src or the browser will block the
script by design.
