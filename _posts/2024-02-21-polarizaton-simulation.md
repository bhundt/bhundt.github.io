---
layout: post
title: "Simulating societal polarization dynamics using Streamlit"
date: 2024-02-21 18:00:00 +0100
comments: false
---
## Introduction

Societal polarization is the phenomenon where opinions on specific topics (ideological polarization) and emotions towards other political groups (affective polarization) within a society diverge over time. While evidence points to increasing affective polarization in countries like the USA the phenomenon of affective polarization is more nuanced in other countries (see ["Cross-Country Trends in Affective Polarization" by Boxell et al](https://www.nber.org/papers/w26669)).

In the paper ["Preventing extreme polarization of political attitudes" by Axelrod et al.](https://www.pnas.org/doi/10.1073/pnas.2102139118#ref-22) a simple agent-based model is introduced in which the authors focus on issue based polarization. The model hinges on three key parameters:

- **Exposure probability**: The likelihood that an agent interacts with another agent holding a differing opinion.
- **Tolerance window**: The extent to which an agent is accepting of another's opinion.
- **Reaction**: The intensity of an agent's shift in position upon encountering another's viewpoint.

Importantly, the amount by which the actor moves is always larger when repulsed by an opinion compared to the case when an actor is attracted to the position of another actor.
Simulation

## Implementation and Simulation

Inspired by the paper I replicated the model in Python. The code is based on a nice framework for agent based simulation called [AgentPy](https://github.com/jofmi/agentpy). To make the model easily accessible I packaged it into a [Streamlit](https://streamlit.io) applicattion and published it on Streamlit Cloud.

You can play around with the model [here on Streamlit Cloud](https://bhundt-polarization-simulation.streamlit.app/).

The paper provides a thorough analysis of the model's implications. One notable takeaway is the potential counterproductive effect of dismantling "filter bubbles." In a society predisposed to polarization, increasing exposure probability could inadvertently accelerate polarization, assuming all other parameters remain constant.

## Summary and Disussion

All models are wrong, but some are useful.Is this useful? Well..from the technical perspective it was fun replicating the model and working with AgentPy. It was also the first time I built a Streamlit app which was also a nice surprise in how easy and simple the whole development and deployment process was.

The model's societal implications, however, are more ambiguous. It offers a plausible explanation for how social media might expedite polarization, as discussed. Yet, the model also posits a debatable assumption:

> Unless the actor is already near an extreme, an interesting effect of this rule is that repulsion moves actors farther than attraction does. [...] Repulsion is less likely than attraction, but it leads to greater movement when it does occur.

The rationale for this assumption remains unclear.

All in all a fun exercise.

**Code** [https://github.com/bhundt/polarization-simulation](https://github.com/bhundt/polarization-simulation)