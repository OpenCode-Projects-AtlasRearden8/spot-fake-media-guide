# 05: Deepfake Video

Video carries the most authority of any media — more than an image, more
than a voice note — and for many years that authority was well earned:
filming required a camera pointed at reality. Generated video is now good
enough that short clips can be entirely invented, faces can be swapped onto
real bodies, and a single "leaked" clip can shape an opinion before the
correction exists.

This chapter is about watching a clip the way an editor does: checking the
physics of mouths, the seams of faces, and the story around the footage.

## When to worry (and when not to)

Worry level rises with three ingredients: **a famous face**, **a striking
quote or act**, and **a suddenly-shared urgency** ("before it's deleted!").
A clip with none of those deserves no forensic pass. A clip with all three
deserves the five minutes — and chapters 06 and 08.

## The watch-tells (in order)

1. **The lip-sync problem, specifically on P, B, M.** These "labial"
   letters need closed lips. On a face-swap, you often see the mouth move
   during them anyway — "my son" whose lips flap open on the "m". Zoom on
   the mouth during speech and look for phonemes (sounds) with no matching
   mouth shapes: lips that never quite close for an "m", teeth that never
   show on an "s".
2. **The face-edge seam.** Where a face was swapped or generated, the
   boundary is at the hairline, jaw, and ears: hair that
   shimmers when the head turns, ears that change shape between moments,
   a jawline that "swims" a few pixels during talk, skin that gets suddenly
   smoother over the cheekbones-and-hair border.
3. **Eyes and glasses.** Uneven blink rates (both eyes, or one eye
   blinking strangely), highlights in the eyes that don't match any light
   in the scene, eyeglass reflections that show a different room than the
   camera sees. Glasses are the trouble spot generation tools most often
   get wrong, so this check earns its keep.
4. **Hands and held things.** Same as photos (chapter 02): fingers that
   rest at the wrong angle, phones/cups/mics that melt into palms or change
   hands; jewelry that flickers shape as a hand moves.
5. **Body-and-background agreement.** As the subject moves, the
   background should respond consistently: fence posts, doorframes, flags,
   crowd. In many generated clips, background geometry bends around the
   head, a pole passes behind then briefly in front of an arm, ripples of
   distortion trail fast motions.
6. **Lighting across the clip.** Light should be one person's weather:
   shadows falling consistently, glow on the face matching glow on the wall.
   Watch for a face whose brightness stays constant while the background
   brightness changes — the paint of "different footage stapled together."
7. **The too-short, too-blurry problem.** Generated clips are *usually*
   shorter than the claim they support, and they arrive cropped, re-encoded,
   and tiny. A clip claiming "here is proof of the thing" that refuses to be
   longer than eleven seconds, higher than 480p, or any shape but vertical
   is functioning in exactly the range fakes are most comfortable in.
   Ask: is the *claim* small compared to the *resolution*?

:::tip The slow-motion trick (30 seconds)
Open the clip full screen on a phone, tap the screen → playback speed →
0.5x (or 0.25x on many players). At half speed, the physics tells become
much easier to see: mouth-lag on labials, the face-edge shimmer, jewelry
problems, the background warping during arm swings. It's the easiest
upgrade to your eyesight we know of.
:::

## The keyframe move (for reverse-searching video)

Video is just a stack of photos, so chapter 06 applies: find a bright,
distinct moment (a face on its own, a clear sign, an unusual object),
**pause there, take a screenshot, and reverse-image-search that frame.**
Often the search finds the *original video's* versions — with earlier dates
or a different story attached (shallowfake!). The frame search beats the
whole-video search almost every time.

## The shallowfake slot for video

Real video with the wrong story is still the internet's most popular fake.
Before you dispute or share any clip, ask the two shallowfake questions:

1. **When** was this filmed, and can the post prove it ("as seen on stream
   X at minute Y" beats vibes)?
2. **Where** was it filmed — same event as claimed, or another one that
   shares a look (same disaster, different year)?

This is above all a *hurricanes happen* pattern: a real clip from a past
event gets rebadged as the current one, spreading twice as fast because it's
genuine footage. When the pixels are real and the context is wrong, the
correction writes itself: "this is real footage, but from [when/where], not
the event claimed."

## A fair note: what a real "bad" video looks like

Real street-level video is shaky, out of breath, off-center, blown out by
contrast, half blocked by a stranger's elbow: authentic filming of an
unexpected event is genuinely ugly. Perfectly framed, slowly panned
"suddenly filmed" moments deserve an extra check. But the reverse is NOT
safe to conclude — shaky alone proves nothing (fakes can add shake, and a
lot of real documentation is beautiful). It's two tells or, once again,
the second-source rule.

:::warn Before you accuse
The stakes cut both ways: wrongfully calling a real, harrowing, honest clip
"deepfake! AI!!" hurts the person who filmed it and helps people who want
all cameras doubted. If you notice *one* tell, your next move is more
checking (06, 08), not an accusation. If your verdict is "unresolved," say
only that: "I can't tell. Let's wait for more sources." That sentence
protects everyone, including tomorrow's you.
:::
