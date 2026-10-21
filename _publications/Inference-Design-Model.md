---
layout: post
title: Understanding the inference and design of haptic experiences
description: The Inference-Design Model relates haptic stimuli, sensations, and experiences.
# redirect: https://doi.org/10.1016/j.ijhcs.2025.103598
published: true
date: 20.08.2025
doi: 10.1016/j.ijhcs.2025.103598
publication: International Journal of Human-Computer Studies (IJHCS)
image: inference-design-model-minified.png
year: 2025
---

In this paper, we propose the Inference-Design Model for Haptic Experience, a model that separates three things that haptic research often conflates: the *stimulus* (what a device produces), the *sensation* (what a person feels), and the *experience* (what the touch means to them).
The model links the three through two opposite processes: *inference*, which people use to interpret a sensory environment, and *design*, which designers use to shape it.
We ground the model in philosophy, neuroscience, psychology, and HCI, and use it to derive six observations about how haptic experiences arise and how they can be studied and designed.
The model is exploratory and idealised. It is a thinking tool, not a predictive theory.

# The Inference-Design Model
Inference is the cognitive process through which a person turns a stimulus into a sensation and, in turn, into an experience. We distinguish two levels:
- *Low-level inference* (stimulus to sensation) answers "how does it feel?", for example, a buzz on the wrist.
- *High-level inference* (sensation to experience) answers "what does this feel like?", for example, a calming or an anxious touch.

![The Inference-Design Model for Haptic Experience](/assets/images/publications/inference-design-model-minified.png)
<small>*Figure. The Inference-Design Model for Haptic Experience. Inference (blue) runs from stimulus to sensation to experience; design (red) runs in the opposite direction.*</small>

Design is the inverse process. Low-level design targets sensations, and high-level design targets experiences. 
Because designers can only configure stimuli, they design *for* experiences rather than directly creating them.

We illustrate the model with a running example of two researchers building a wrist-worn vibrotactile device that conveys the anxiety of others during conversation.

# Six Observations
- *Sensations differ from experiences:* Sensations are properties of what is touched, while experiences are situated, embodied, and personal.
- *Sensations are constrained, experiences are dynamic:* One stimulus can evoke many different experiences. We use an "experience funnel" to show how technology and methods can narrow this range.
- *Touch is phenomenally special:* Touch gives a double experience of self and other, and differs between active and passive touch. Ethics, such as sensory autonomy and consent, should therefore be part of the design process.
- *Methods are inadequate for high-level inference:* Psychophysics suits low-level inference, but understanding experiences requires methods such as micro-phenomenology, interviews, and in-depth qualitative work.
- *Haptic design configures stimuli, not experiences:* The same stimulus can result in different experiences, so designers need to design for experiences.
- *Context shapes experience:* We propose *narrative haptic design* and *narrative congruence*, where the haptic stimulus fits the story it is part of.

# Limitations and Future Work
The model does not explain illusions such as the thermal grill and rubber hand illusions, and it does not yet represent context or past experience.
Open questions include where the boundary between sensation and experience lies (is pain a sensation or an experience?) and how variable experiences are at the top of the funnel. 
Next steps include empirical validation through neuroscience and phenomenology.

Read the full paper here: [10.1016/j.ijhcs.2025.103598](https://doi.org/10.1016/j.ijhcs.2025.103598).

Cite this work using the following:
```
@article{10.1016/j.ijhcs.2025.103598,
 author = {Dalsgaard, Tor-Salve and Bergstr{\"o}m, Joanna and Hornb{\ae}k, Kasper},
 title = {Understanding the inference and design of haptic experiences},
 journal = {International Journal of Human-Computer Studies},
 volume = {204},
 pages = {103598},
 year = {2025},
 doi = {10.1016/j.ijhcs.2025.103598},
}
```