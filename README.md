# The Disney Trip

Birthday invitation site for Jacob's 30th at Disneyland Resort. The group days are September 19 and 20, 2026.

Single self-contained page. No build step, no dependencies, no external assets.
Open `index.html` directly, or serve the folder from any static host.

## What it does

- **Name gate.** Visitors type a first name. If it matches the guest list they're let in,
  and the browser remembers them so they never type it again.
- **Fireworks welcome.** A canvas fireworks show plus a full-screen "Be Our Guest" on the
  first successful sign-in per device. Skipped on return visits and when the visitor has
  reduced motion turned on.
- **The invite.** Two birthday asks (castle photo, group lunch), loose day-by-day plans,
  and park gotchas for those dates.
- **Prints clean.** Flips to black on white so it doesn't eat a toner cartridge.

## Editing the guest list

Near the bottom of `index.html`:

```js
var ROSTER = [
  "Jacob",
  "Mama Weber"
];
```

Add the rest of the first names there. Matching ignores capitalization and extra spaces,
and accepts either a full listed name or just its first word.

## Note on the gate

This is a doorman, not a lock. The names live in the page source, so anyone determined
could read them. Fine for family. Do not treat it as security.

## Credits

`castle.jpg` is a Pexels photo by Poppy Martinez, free to use.
