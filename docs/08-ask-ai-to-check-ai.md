# 08: Ask AI to Check AI

There's a symmetry here worth savoring: the fastest free second opinion on
a suspected AI image is... another AI. Not required — but a chat assistant
that can look at images can find a lot, when you ask the right questions,
and it turns checking from a chore into a conversation. Think of it as a
colleague in a different room: it saw the picture fresh, without your hopes
attached.

(What you must *not* paste anywhere is its own subject — personal
documents, your own photos you wouldn't hand a stranger, intimate images
of anyone. The careful version of that habit lives in *The Privacy Comfort
Handbook*. Hard rule for this chapter: never upload anything sensitive to
a tool you don't trust.)

## Recipe 1: The tell-spotter (for images)

Upload the image (a *file*, when you have it — screenshots suffice only if
a bigger original doesn't exist), then try:

> Look at this image like a forensic photo examiner would. Zoom in on
> hands and anything they're touching, any text, reflections, shadows,
> and the edges where subjects meet the background. List anything that
> looks physically impossible or generative, with as much specificity as
> you can ("top-left, third finger"). Then say what evidence would
> convince you the image is genuinely real.

Two things earn their keep in that prompt: **"with as much specificity as
you can"** (forces it to point at places, not vibes — you can verify the
pointing with your own zoom) and **"what evidence would convince you
[the opposite]"** (which fights the yes-person problem discussed below).

## Recipe 2: The source-tracer (for screenshots and audio/video claims)

You can't always hand it the pixels, but you can hand it the words:

> Here is a claim forwarded to me in a group chat. What's the fastest way
> to find out where it originated? Give me: (1) two exact search phrases
> in quotes I should try, (2) whose account or page the claim would appear
> on if it were real, and (3) what kind of site would have reported on it.

It's remarkable how often the reply seeds exactly the search you needed.
Even better: run the suggested searches, then bring your findings *back*
to the assistant and ask it to interpret what you found.

## Recipe 3: The outrage-meter (for text)

Fake content wants to *move* you first and inform you second — chapter 01's
inverse lever. Give the copy to the assistant:

> Read this post. What does the author want me to feel and do after
> reading it? Which words are doing the emotion work?
> If it were false, what facts would it be hiding?

It's like having a version of yourself that doesn't have the feelings.

## What AI can't reliably do (read this section twice)

- **"Is this AI-made?" detectors are weak in both directions.** Yes, some
  tools claim to detect generated images; independent tests show them
  missing the newest generators *and* flagging real photos. Neither
  mistake is acceptable when it comes out of you as a confident verdict.
  Machine detectors are (currently) one more signal — never the judge.
- **Assistants hallucinate tells.** A chatbot can absolutely tell you
  "the shadows are inconsistent" with quiet confidence about a photo whose
  shadows are fine. It makes stuff up, just like any other confident
  friend; ask it to point to *where* in the image, then verify the
  pointing with your own eyes (recipe 1 is built that way on purpose).
- **It's a two-way street for the newest fakes.** Your knowledge
  has a training-date; so does the assistant. Newer generations escape
  widely-known tells. That's why the durable checklist in chapter 10 runs
  *source, zoom, search, label* — none of which rely on a specific
  generation being weak.

## The prompt that makes AI useful for checking: "what would change your mind"

A single habit makes any assistant more reliable as a checker. After it
gives you an opinion, ask:

> How confident are you, one to ten? And specifically what evidence would
> move you by two points?

Then, critically, do a round of its listed evidence. You've just converted
a vibe into a research plan — which is what every good second opinion really
is, AI or human.

:::note Models are colleagues, not referees
Ask two different assistants the same check and they'll disagree; ask the
same one twice and it might too. None of that is failure — the goal was
never "the machine decides." It's that the machine gives you *things to
check*, faster than the internet from scratch. Your verdict stays yours, and
"unresolved" (chapter 10) stays a legitimate ending.
:::
