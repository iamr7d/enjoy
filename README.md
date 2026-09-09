# JOY — Artificial Viewer

A closed-loop artificial observer that watches film. It receives only a foveated percept, weighs
bottom-up salience against a vision-language model's reading of the scene, keeps a history of
where it has just looked, selects its own fixation, and then perceives the world from wherever
that choice left it.

**The central result is a dissociation.** A low-capacity state-dependent arbitration policy
improves the prediction of human fixation locations by 0.0099 bits per frame, positive in five of
five folds. The same policy, put in charge of the loop, has a median disadvantage of 0.919 bits
and wins on three of eight held-out clips. Getting better at predicting gaze did not make it
better at looking.

MRes Creative Computing, Creative Computing Institute, University of the Arts London.

## What is in here

This is the **demo site only**. It is static and self-contained.

| file | what it is |
|---|---|
| `index.html` | the project page |
| `thesis.html` | the thesis |
| `proposal.html` | the PhD proposal |
| `presentation.html` | the presentation script |
| `figures/` | figures, each generated from a stored result file |
| `hero_stack.png` | one Sintel frame through the viewer's four stages |
| `eye-hero.jpg` | header illustration, generated, credited in CREDITS.md |
| `viewer.html` | how to run the interactive viewer locally |

No research code, datasets or model weights are included. The interactive viewer is not hosted
here; see `viewer.html` for why and how to run it.

## Viewing it

Open `index.html`, or serve the folder:

```
python -m http.server 8000
```

## Credits and limits

See [CREDITS.md](CREDITS.md). In short: the hero image is built from *Sintel*, which is
Creative Commons; two figures that reproduce broadcast footage are withheld from this public
copy and appear only in the submitted thesis.
