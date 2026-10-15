# The Lolli Showcase 🎉🇮🇹

A one-page birthday game show that ends by revealing the trip to Italy. It's all in `index.html`. Sounds and music are generated in the browser, so there are no audio files and nothing to install.

## The flow (about 4–5 minutes)
1. **Start**: tap "Start the Show" (this turns sound on)
2. **Come on down, Lolli!**: fanfare, applause, confetti
3. **Round 1, Pick a Door**: every door is a dud (socks, DMV, toaster). Sad trombone. Consolation prize: ☕
4. **Round 2, Trivia**: 3 questions. Every answer wins a clue: 🍕 🍝 🛵
5. **Round 3, Scratch-offs**: Chicago → Lolli + Poppi → … **Cleveland?!** (buzzer)
6. **The Showcase**: drumroll, curtains open… **A BRAND NEW CAR!** Then a record scratch, then **WRONG ENVELOPE**
7. **Golden envelope** → curtains → drumroll → **ITALIA!** Boarding pass, the trip highlights (Vatican, Colosseum, pasta class, Amalfi Coast), the packed suitcase, your message, and music

## Customizing
Open `index.html` and edit the `CONFIG` block at the top of the `<script>`:
- `partner`: what the family calls your dad (currently "Poppi")
- `depart` / `return`: trip dates on the boarding pass
- `trivia`: replace the questions and answers with inside jokes. `correct: null` means every answer wins. Use `0`–`3` to mark a real right answer (wrong answers still get the point).
- `themeLine`: update it if you change the trivia prizes
- `doorPrizes`, `fakeDestination`: the misdirects
- `photo`: put a picture in a `photos/` folder and set `photo: "photos/lolli-and-grandpa.jpg"`
- `message` / `signoff`: your note on the final screen

## Testing shortcuts
Add `?jump=doors`, `?jump=trivia`, `?jump=scratch` or `?jump=showcase` to the URL to skip ahead. Don't send her those links!

## Publishing on GitHub Pages
1. Create a new repo on github.com. Free Pages needs it to be **public**, so pick a name that won't spoil anything, like `lolli-showcase`.
2. Upload `index.html` (and the `photos/` folder if you have one): **Add file → Upload files → Commit**.
3. **Settings → Pages → Source: Deploy from a branch → `main` / root → Save**.
4. After about a minute it's live at `https://<your-username>.github.io/lolli-showcase/`.

## On the big day
- Open the link on a laptop hooked up to the TV, turn the volume up, and press **F** for full screen.
- **Space / Enter / →** advance to the next step, so whoever's at the keyboard can drive while she calls the shots. **M** mutes.
- On a phone, turn off the silent switch (iPhone) or the sound won't play.

