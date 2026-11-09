# Keepsake: Google Stitch design brief

Paste the "Master prompt" into Stitch first, then paste each "Screen prompt" one at a time. Upload `keepsake-mockup.html` screenshots as reference images if you want Stitch to match the layout.

## Master prompt (design system)

Design a web app called **Keepsake**, a calm place where everyone at an event drops their photos and videos, and AI turns them into things worth keeping. Platform: responsive web, desktop first, 1440px wide.

**Feeling:** light, airy, minimal, quietly creative. Like a well-lit gallery, not a party app. No pink, no purple gradients, no cream or beige.

**Color**
- Background: mist `#F5F7F8`
- Surface (cards, panels): white `#FFFFFF`
- Ink (text): deep ink-blue `#172330`
- Muted text: `#6B7885`
- Hairline borders: `#E3E8EC`
- Primary accent: cobalt `#3558F0` (buttons, active states, links)
- Secondary: sea-glass `#CFEBE1` (selected tiles, soft highlights)
- Signal: sun `#FFC94A`, used ONLY for AI face-detection markers, so it always means "AI found a person here"

**Typography:** Bricolage Grotesque for headings (semibold, tight tracking); DM Sans for body and UI. Sentence case everywhere. No all-caps labels.

**Shape and depth:** 14px radius on cards, 999px on chips and buttons, 6px on photo thumbnails. Almost no shadows; use 1px hairline borders. Generous whitespace, 8px spacing grid, content max width 1200px.

**Components:** pill buttons (primary filled cobalt, secondary outlined), segmented tabs, face avatar chips with a count, photo grid with masonry layout, side panel for tools, toast messages in plain language ("Sorted 214 photos into 9 people").

**Voice:** plain, active, specific. Buttons say what happens: "Sort photos", "Make collage", "Use this style".

## Screen 1: Event home

Top bar: Keepsake wordmark left, event name "Meera and Dev's wedding" centre, avatars of contributors and a "Invite people" button right.
Below: a large quiet hero card with the event cover photo, date, and three stat numbers (photos, videos, people). Under it, three tool cards in a row: **Sort by faces**, **Make a collage**, **Remix a video**. Under those, an "All uploads" masonry grid with an upload drop zone as the first tile ("Drop photos or connect a folder").

## Screen 2: Sort by faces

Left: scrollable column of detected people as round face chips with names (editable) and photo counts; "Unnamed person 3" style placeholders with a "Name them" inline field. Right: masonry grid of the selected person's photos; small sun-yellow rounded square outlines mark each detected face on hover. Top right: filters (Everyone, Groups, Solo), a "Merge people" action, and a "Download this person's photos" button. Empty state: "Connect a folder or upload photos and we'll group them by person."
Include a privacy note chip: "Face matching stays inside this event."

## Screen 3: Collage maker

Three-column workspace. Left: **Format** chooser as tall selectable tiles: Instagram story (9:16), Instagram post (1:1), Photo frame (4:5 and 3:2), Print poster (A3), Phone wallpaper. Selected tile gets a sea-glass fill and cobalt outline. Under it: layout styles (Grid, Scrapbook, Film strip, Polaroid stack, Mosaic).
Centre: the canvas showing the live collage in the chosen format on a soft grey stage with a zoom control.
Right: "Pick photos" panel with tabs *Auto-pick*, *By person*, *Manual*; a spacing slider, corner roundness slider, and background swatches (white, mist, sea-glass, ink). Primary button: "Make collage". Secondary: "Shuffle layout", "Download".

## Screen 4: Remix a video

Left: a library of shared reference videos as vertical cards with title, creator and a "Remix this" button; a "Share a reference" button above (upload or paste a link). Centre: two phone-shaped players side by side: "Reference" and "Your edit", with a synced timeline underneath showing cuts as small markers. Right: panel "What the AI found in the reference" listing cut count, music beat, text overlays and transitions, with a toggle for each ("Match the cuts", "Use the same transitions", "Keep my music"). Primary button: "Apply to my clips". Below the timeline, a row of the user's clips to drag in.
Make it feel like a simple editor, not a pro timeline.

## Screen 5: Share and invite

Modal: event link with copy button, QR code, toggle for "Anyone with the link can add photos", list of contributors with roles, and "Download everything" button.

## Notes for refinement in Stitch
- Keep one memorable thing: the sun-yellow face markers. Everything else stays quiet.
- Try the dark variant only after the light version is final.
- Ask Stitch for mobile versions of screens 1, 3 and 4 afterwards.
