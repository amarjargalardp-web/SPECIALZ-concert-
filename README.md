# SPECIALZ-concert-
A program where keys trigger stage animations for the projector, with a live phone camera feed.

## Files

| File | Open it on | What it does |
| --- | --- | --- |
| `Special_project_SPECIALZ.html` | the computer driving the projector | All the visuals, the key controls, and the receiver for the phone camera |
| `phone.html` | the phone filming the band | Sends the phone camera live to the computer |
| `index.html` | either | Start page linking to the two above |

## Keys (computer)

| Key | Animation |
| --- | --- |
| 1 | Haze: slow red breathing |
| 2 | Pulse: hard beat flashes |
| 3 | Glitch: sliced, shaking visuals |
| 4 | Strobe: black with a white hit on every beat |
| 5 | Psychedelic: liquid colour warp |
| 6 | Lasers: patterns change every bar |
| 7 | Mirror mountains: silver glass peaks catching a moving light |
| 8 | Signal break: warped bars, tearing, static |
| 9 | Chorus: red glass mountains with lasers from the peak |
| 0 | Hypnotic spiral |
| A | Aurora opening (aurora, stars, white bird). Press A again to ignite the mountains red |
| D | Shard storm: glass shards fly at the audience |
| B / R | Black / solid red |
| **Q** | Eyes: spiral pair |
| **W** | Eyes: giant eye |
| **E** | Eyes: wall of eyes |
| **Y** | Eyes: four eyes (second pair opens underneath) |
| **U** | Eyes: dive into the eye (endless) |
| **I** | Eyes: beat eyes (pop open on every beat) |
| C | Live camera full screen |
| V | Next camera look (Red, Clean, Mono, Noise, Glitch, Mirror) |
| X | Mix the camera over the running scene |
| S | Title slam (screen text or SPECIALZ, then shatters) |
| G | Ghost line, 7 seconds |
| Enter (hold) | Show the screen text |
| Space | White hit; hold for strobe |
| T | Tap tempo |
| H / F | Show or hide the panel / fullscreen |

## Phone camera setup

The phone page needs to be opened over **https** (phones only allow the camera on secure pages), and both devices need internet.
The connection runs through the free PeerJS relay, then goes straight between the phone and the computer.

The easiest host is GitHub Pages:

1. Make this repository public (Settings → General → Danger Zone → Change visibility). GitHub Pages on a private repository needs a paid plan.
2. Settings → Pages → Build and deployment → Source: *Deploy from a branch*, Branch: `main`, folder `/ (root)` → Save.
3. After a minute the site is at `https://amarjargalardp-web.github.io/SPECIALZ-concert-/`.

Then on the night:

1. On the computer, open `https://amarjargalardp-web.github.io/SPECIALZ-concert-/Special_project_SPECIALZ.html` in Chrome or Edge.
   The panel shows a 4-letter code and a QR code. The code stays the same between reloads.
2. On the phone, scan the QR code and allow the camera. It goes live by itself. Keep the phone screen on and the page open.
3. Press **C** to show the phone, **V** to change the look, **X** to mix it over the visuals. The phone shows **ON SCREEN** while it is being used.

The computer panel shows how the phone is connected and how long the picture took.
If it says *via relay server*, put both devices on the same Wi-Fi, or connect the computer to the phone's hotspot, for a faster, steadier link.

No internet at the venue? Use a webcam app instead (iPhone Continuity Camera on a Mac, DroidCam, Camo, Iriun, or Windows Phone Link).
The phone then shows up as a camera on the computer: pick it under **Computer cam** in the panel and choose **Computer cam** as the source.

## If something looks frozen

- The program now ignores the computer's "reduce motion" setting, which used to freeze some scenes.
- The panel shows the frame rate. If a laptop can't keep up, the program lowers its own resolution so the animation keeps moving.
- The claude.ai artifact preview blocks the camera and the phone link. Use the GitHub Pages copy (or a downloaded copy) for the concert.
