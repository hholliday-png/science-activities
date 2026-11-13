# Unit 8: Tectonic Plates · Game Hub

Six self-contained pages. No accounts, no saved data, and no outside connections:
each page carries everything it needs inside the file.

| File | What it is |
|---|---|
| `index.html` | Unit 8 home page that links every game (share this link with students) |
| `fault-lines-quest.html` | Story quest: 8 cases, cards, Plate Lab, Megaquake boss |
| `volcano-defense.html` | Strategy game: answer to earn rock, build defenses, survive 10 waves |
| `escape-room.html` | Escape the Magma Chamber: 4 puzzle rooms |
| `simulators.html` | Quake Locator, Volcano Builder, Stripe Recorder (add `#quake`, `#volcano` or `#stripe` to the link to open one directly) |
| `case-files-challenge.html` | The original, longer Case Files for test review |

## Putting it on GitHub Pages
1. Copy the whole `unit8` folder into your GitHub Pages repository (keep the files together in one folder).
2. Commit and push.
3. The student link is your Pages address followed by `/unit8/`, for example `https://YOUR-USERNAME.github.io/YOUR-REPO/unit8/`.

To link straight to one game, use its file name, such as `.../unit8/volcano-defense.html`.

## Visual refresh v2 (Nov 2026)

A second polish pass on top of the v2 files. Nothing about the games
themselves changed — same questions, answers, scoring, and outcomes.
Only presentation, layout, and extra interaction chrome.

### Fits a normal 16:9 screen
- Desktop (laptops, Chromebooks, projectors) now uses the full width:
  the 1280px centered column is gone on the quest and case-files pages,
  and the side panels widen to 350px on screens 1400px and up.
- The quest and case-files story pages got the same one-screen
  treatment the other games already had: header, a slim progress strip,
  and the play area fill the viewport with no page scrolling at
  1920×1080 or 1366×768. Chat bubbles, diagrams, and math cards widen
  to 720px on big screens. Phones (under 900px) still scroll as before.

### Looks better
- Hub: game tiles got gradient icon chips, a gold glow on the
  "Start here" tile, and a shine sweep on hover; hero type grows on
  wide screens.
- Quest / Case Files: a thin gold progress strip under the header
  (cases closed, dead ends mapped), deeper shadows on the chat column,
  and figures (diagrams) that glow gold on hover.
- Volcano Defense: a row of 10 wave dots under the stats (done / current
  / upcoming) and a gold-framed scene.
- Escape Room: the current door pulses, the room panel has a gold-framed
  shadow, and seismograph screens brighten on hover.
- Simulators: each simulator's canvas gets its own accent frame —
  teal for Quake Locator, magma orange for Volcano Builder, violet for
  Stripe Recorder.

### More interactive (no game logic changed)
- Hub: hover or focus a tile and Terra tells you what that game is;
  keys 1–5 open the games; clicking a tile bursts a sparkle.
- Quest: Terra now coaches from the side panel and reacts — cheering
  on a closed case or a 3-answer streak, looking worried at a dead end;
  hovering the Plate Lab / Megaquake tiles gets a tip; clicking a
  diagram opens it big in a modal.
- Case Files: this page never had the Terra/flair kit, so it got one —
  Terra coaches from the side panel, reacts to closed cases and dead
  ends, star-bursts on a closed case, a 🗣️ read-aloud toggle in the
  header, diagram zoom, and hover tips on the case cards.
- Volcano Defense: keys 1–6 jump to the build tools (Enter places one);
  a wave where every hazard is blocked ends in confetti.
- Escape Room: Arrow Up/Down on a focused dial spins it; tapping the
  room picture makes a little sparkle.
- Simulators: keys 1–3 switch simulators; finishing every mission in
  a simulator gets a Terra cheer and a star-burst.

### Notes
- Still zero outside connections: no web fonts, images, CDNs, or fetch.
- Every file is still self-contained; the six files link to each other
  by filename, and the simulator deep links (#quake, #volcano, #stripe)
  still work.
- All changes are in appended, commented "VISUAL POLISH v2" blocks, so
  the original code is easy to find and revert.
