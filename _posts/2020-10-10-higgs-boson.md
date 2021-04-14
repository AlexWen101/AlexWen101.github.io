---
layout: post
title: "The Higgs Boson"
author: "Alex Wen"
categories: journal
tags: []
image: atlas-higgs-event.png
---

The joint discovery of the Higgs boson at CERN by two large experiments - ATLAS and CMS - in 2012 was one of the defining triumphs of modern physics. The whole story illustrated a beautiful iteration of research, spanning almost everything: theory, technology, experiment, and human cooperation all came together to enable the discovery of the one of the most important particles we know of. You may have heard the Higgs boson referred to as the "God particle" (though many high-profile physicists like Peter Higgs [abhor](https://www.theguardian.com/science/blog/2009/may/29/why-call-it-the-god-particle-higgs-boson-cern-lhc) the term) which, more than anything else, is a testament to the popular curiosity and excitement surrounding a groundbreaking physical achievement.

The focus of the ATLAS experiment has since momentarily diverged from discovery, to one of measurement. We found the Higgs, but now we want to know more - especially its mass. But what is the Higgs, really? Why do we even care about finding it, so much so that we need an international collaboration and a machine that [weighs as much as](https://atlas.cern/discover/detector) the **Eiffel Tower**?

## Particle Physics in a Nutshell

Particle physics is the study of the smallest, most elementary particles we know of, on the extreme end of the size scale of objects in the universe. Because of the physical forces we need to overcome, and how hard it is, to isolate, create and study elementary particles, much of particle physics is intrinsically entangled with machines called particle accelerators that apply huge amounts of energy to particles so they can be collided, undergo certain reactions, and studied by waiting detectors. Due to this, "particle physics" is often interchangeable with "high energy physics."

Currently, we have a theory called the Standard Model describing virtually all of known particle physics. In science, a "theory" is a explanation of nature that's falsifiable and rigorously tested and analyzed; a "theory," should an idea have this grand and particular title, is the most reliable kind of scientific knowledge out there. Far from the vernacular denotation of "hunch" or "opinion," the theory that is the Standard Model has been under relentless experimental siege for decades, and has tenaciously withstood every experimental test. As far as we know, the Standard Model is "correct," *at least* as an excellent approximation for perhaps an even more elementary theory or reality.

The Standard Model is, crudely put, a classification of all known elementary particles, and a collection of laws that govern their interactions. Intuitively, we can understand the Standard Model as a "zoo" of particles and a description of the interactions that exist between them.

<center><img src="{{ site.github.url }}/assets/img/standardmodel.png" alt="sm" width="450"/></center>
<center><i>A representation of the Standard Model - all the elementary particles we know of (plus some more antiparticles),</i></center>

The most fundamental distinction we make between different particles is based on their spin angular momentum, which is an intrinsic, immutable property of the particle - like an adult's height. It's a defining feature of particles that dictates how it behaves, and thus physicists find it very useful to classify particles based on their spin. We call particles with a half-integer (numbers like 1/2, 3/2, 5/2, 69/2, etc.) spin *fermions*, and those with an integer (1, 2, 3,...) spin *bosons*. From some [deep and complicated results](https://en.wikipedia.org/wiki/Spin%E2%80%93statistics_theorem#:~:text=In%20quantum%20mechanics%2C%20the%20spin,spin%20or%20half%2Dinteger%20spin.), every particle in the world as we know it must have either a half-integer or integer spin.

The fermions are probably familiar to many people. They include the quarks, which make up popular bits of matter like protons and neutrons, which in turn make up atomic nuclei. They also include electrons and neutrinos, other parts of matter you've probably heard of.

The bosons are where things get a little strange. Elementary *vector bosons*, or bosons with a spin of 1, are sometimes understood as "force carriers" - they're associated with a physical force and are often seen when that force is at play. The photon - light - is one such vector boson that happens to be massless, and "carries" the electromagnetic force. The gluon, also massless, "carries" the strong force, and the W and Z bosons "carry" the weak force. As of yet there's mention of the fourth fundamental force, gravity - a telltale sign that the Standard Model isn't quite perfect yet.

The Higgs boson is a elementary *scalar boson*, or a boson with a spin of 0. The story of the Higgs boson begins with a series of baffling experimental observations.

## The Higgs Boson

If you look carefully at the vector bosons, you'll notice that the photon and gluon (there are actually 8 types of gluons, but that's a story for another day) are each massless. However, the W and Z bosons are not - they were measured in 1983 to have rather unmistakable and significant masses [1]. This will turn out to be a major problem - but to understand why, we need a little background first.

### An Aside on Lagrangians

In physics we use mathematical functions called [Lagrangians](https://en.wikipedia.org/wiki/Lagrangian_mechanics) to describe stuff. It's the bread and butter of mechanics - with them, we can often find the equations of motion of some particle or object, and completely determine how things will behave. For example (if we neglected relativity) the Lagrangian $\mathcal{L}$ for a particle is

$$\mathcal{L} = T - V, $$

the kinetic energy $T$ less the potential energy $V$, each a function of the position and velocity of the particle. This is an easy enough quantity to understand - but the catch is that $\mathcal{L}$ satisfies a set of differential equations called the Euler-Lagrange equations - and plugging $\mathcal{L}$ into those equations gives us the equations of motion that completely describe how the particle moves (the original goal of physics!). All in all, $\mathcal{L}$ provides critical information on how a system behaves.

However, the Lagrangian is a purely mathematical construct we use to help describe reality. Based on reality, we can *impose* specific conditions on how the math *must* behave. For example, we can *demand* that the Lagrangian doesn't change under certain kinds of mathematical transformations to its terms. However, if we impose all these conditions on the math, new things drop out.

Maybe a simple toy example will help - consider the following equation, with $y(x)=5$:

$$ L = \frac{d}{dx}y(x) = \frac{d}{dx}(5) = 0, $$

and now suppose that we *demand* $L$ must not change, if we change $y(x)=5$ to $y(x)=x^2$. Okay, well since

$$ \frac{d}{dx}y(x) = \frac{d}{dx}x^2 = 2x, $$

if we're to not let $L$ change, we'd have to add a new term, $-2x$:

$$ L = \frac{d}{dx}y(x) - 2x = \frac{d}{dx}x^2 - 2x = 2x-2x = 0. $$

Conclusion: by *demanding* that $L$ doesn't change while we change $y(x)=5 \rightarrow y(x)=x^2$, we end up with an extra term of $-2x$ in $L$:

$$L \rightarrow L - 2x. $$

This is crudely analogous to how vector bosons were theorized. We can take a certain Lagrangian, and then *demand* that it be something called [locally gauge invariant](https://en.wikipedia.org/wiki/Gauge_theory) - loosely, that the Lagrangian not change under some operation (analogous to setting $y(x)=x^2$ in our example) that depends on an arbitrary function of space and time. Doing this, we saw extra terms (like the $-2x$ in our example) drop out. These terms described *vector fields* (a whole new can of worms), but whatever - the key is that these fields were attributable to the different vector bosons - the photon, gluon, and W/Z.

The caveat was that these new fields and bosons that fell out of imposing local gauge invariance on Lagrangians had to be massless (certain terms represent the mass, and these are missing) - so for the photon (electromagnetic force) and gluon (strong force), both massless, their prediction and experimental study was smooth and predictable.

The problem was, the W and Z (weak force) were also supposed to be massless in the same way. That's a huge no-no, if your detector had just confidently measured their (non-zero) mass!

### The Actual Higgs Boson

We've arrived at a point where theory for the weak interaction (we call this kind of theory a *local gauge theory*) disagrees with experiment - and unless the theory can be modified to explain why, it has to be thrown out. Its breakdown would mean a fatal blow to the Standard Model.

A fix was proposed by, among others, [Brout, Englert, and Higgs](https://home.cern/science/physics/higgs-boson) so it could describe why the W and Z had mass.

Exploiting how Lagrangians tend to be written, and by changing the notation, we can write Lagrangians in a form that introduces a mass term, but also induces what's called *spontaneous symmetry breaking*: a symmetry had been lost just by virtue of us writing the Lagrangian differently, and us choosing a particular ground state of it to work with. An example of a symmetry that can be "broken" is an even function: it may lose the property that $f(x)=f(-x)$ if we define $x$ differently. It's fundamentally a clever and equivalent re-writing of the math's format.

Using this, and some more mathematical hokey-pokey, including exploiting more gauge invariance, we can end up with a Lagrangian that permits the W and Z to have mass. We can *manufacture* mass terms for the W/Z; but like before, things tend to drop out of equations when we impose restrictions on them. Doing so created a new massive scalar field, and a corresponding scalar boson. The Higgs!

*In summary: the (unexpectedly) nonzero masses of the W and Z require modifications to the theory of the Standard Model; these new mathematics can explain the nonzero masses, but they necessarily also predict the existence of a new gauge boson, the Higgs. To check the theory, we should look for the Higgs boson.*

### What?

All of this may seem like pulling things out of a hat - but remember that we are only constructing a piece of *math*. Based on our observations, and the assumptions about reality that we think are true, we can *demand* the math to behave a certain way.

To this end we can write our math in any form we like and use any variables we want - and the math can still be *true and correct* - but certain ways we write math can give us evident *physical insights* depending on how the math behaves (like, for example, seeing certain terms drop out of the Lagrangian), and how we've written it. In physics, math is a fit to reality. At the end of the day we can have endless math that is *correct*, but only a smaller subset that is *descriptive.*

We massage and coax the math to fit observation, but along the way the math might reveal some things that we *haven't* observed yet. If we're right about the theory of the weak force, then we should try to test it. Since it predicted a massive boson, the Higgs, can we find it?

Well I'm glad someone asked. Remember that machine I mentioned, which weighs as much as the Eiffel Tower?

## The ATLAS Detector

Behold:

<center><img src="{{ site.github.url }}/assets/img/atlas-with-people.jpg" alt="sm" width="450"/></center>
<center><i>One end of the ATLAS detector with people (who I don't know) for scale.</i></center>

ATLAS stands for "**A** **T**oroidal **L**HC **A**pparatu**s**," with LHC standing for Large Hadron Collider. The LHC is the world's most energetic particle accelerator, and it directly shoots two beams of near light-speed protons at each other. When they collide, a whole slurry of reactions occur - because the energy is so high (the protons are fast), new massive particles can be created that normally wouldn't be seen naturally. This causes an explosion of particles going all directions outward. To identify those new particles, we have to construct layers of arrays of large, bulky particle detectors that surround the collision point. Hence ATLAS looks more like a barrel:

<center><img src="{{ site.github.url }}/assets/img/atlas-diagram.jpg" alt="sm" width="650"/></center>
<center><i>ATLAS diagram showing the main barrel-shaped nest of detectors. The proton beams come in from the ends and collide in the center.</i></center>

It's a little bit like trying to outwit a magician; to get to the bottom of their devious tricks, we can invite a group of friends to surround them and watch them from all directions, so that we catch everything they do behind their back. It comes at a price, though. ATLAS has to operate around 100 million electronic channels and is wired up by 3000 km of cables [2] - it needs to be comprehensive, sensitive, and repeatedly handle particles from around a billion proton collisions *per second* - after a bunch of filters, that still generates around 3200 terabytes of data per year. This is as of 2011, right before the Higgs discovery - present-day ATLAS is bigger and more sensitive, with many more upgrades.

Every once in a while, a proton collision will have the energy and luck to generate a Higgs boson. It then typically decays soon within ATLAS near the collision point. One way it decays is via the channel
$$ H \rightarrow ZZ \rightarrow 4 \mu, $$
which means that the Higgs boson decays into two Z bosons, and then these in turn each decay into 2 muons (every particle involved is elementary). So the game (for this decay channel) is to find sets of 4 muons that all come from the same point (or "vertex"). There are several other ways the Higgs can decay (and we do use those data too), but this mechanism is especially prone to detection, and less susceptible to false positives from other noise that we don't care about. So it's a good example to talk about.

## The Analysis

Once we've found a bunch of data (i.e. sets of 4 muons we call "events") we think are probably Higgs, we need to check if they have the theorized Higgs properties: for example, does it have zero spin? Is the mass reasonable? And so on.

Now the big analysis problem is that *many* other physical reactions ("background") may produce 4 muons that have nothing to do with the Higgs. They'll look suspiciously like the Higgs signal we want.

The key is that we *know* all the background events and the physics behind them, so we can model them and predict what their distribution of mass will look like. In following plot, the background events we know of are in solid red and purple - if we just measured all the 4 muon (technically the plot has other lepton channels too) in the 80-200 GeV mass range, we *know* that we should see the this distribution. However, on the plot you'll see a little light blue peak at around 125 GeV. It looks distinct from the background - that's the predicted addition of Higgs events to this mass distribution, assuming one possible Higgs mass. Lo and behold, when we look at the real data (the black dots), what do we see? A generally good fit to the prediction, but more importantly, a little peak exactly where the Higgs was anticipated to be, fitting to that little light blue peak.

<center><img src="{{ site.github.url }}/assets/img/HtoZZto4lchannel.jpg" alt="sm" width="400"/></center>
<center><i>In a histogram of mass, we model all the background (red and purple) and the Higgs signal (light blue). We discover that our data (black dots) is a good fit. Figure from [3].</i></center>

This data tells us that there's an unaccounted-for abundance of events right near where the Higgs mass could be, which fit the predicted Higgs mass distribution well. This astounding agreement between the data and theory, and the clear presence of a peak in events, suggested that something new, unusual and exciting was going on. The confirmation of the Higgs properties - zero spin, anticipated mass, etc. strongly suggested that it was indeed the Higgs we found.

Furthermore, statistical tests were done and enough data was collected to make sure that the discovery was indeed from a specific process (a Higgs decay), and not just due to random chance. If you're familiar with p-values in science, particle physics discoveries conventionally require a "$5\sigma$" p-value of around $0.0000003$ to be significant - in other words, if we're $5\sigma$ confident, then there's a $0.0000003$ probability (a $0.00003\%$ chance) that our observation occurred by random chance, and not caused by something special like the Higgs. Equivalently - there's almost sure confidence that our result is *not* due to chance!

Still not convinced? At the same time, another huge barrel-shaped experiment like ATLAS, called CMS (Compact Muon Solenoid) was also trying to find the Higgs on the other side of the LHC, using similar techniques. They found the *same results*: a statistically-significant zero-spin boson in the 125 GeV mass area. This was the nail in the coffin; the joint discovery of the Higgs, with two completely independent and technologically distinct experiments, was indisputable and overwhelming evidence for the existence of the Higgs boson.

## The Result

After all that work, this is the moment where you're allowed to say that you've "found" the Higgs, and hold a huge press conference to thunderous applause (a rare sight in physics research):

<center><img src="{{ site.github.url }}/assets/img/higgs_celebration.jpg" alt="sm" width="550"/></center>

The discovery was monumental. It confirmed the theory of why the W and Z bosons could have mass, and preserved the integrity of the Standard Model. It also placed an initial value on the Higgs mass - around 125 GeV - and this value would be very important, since many other physical theories will interact with it. If your theory didn't come up with this Higgs mass, you had to tweak it or throw it out; if your theory was dependent on this mass, then you could make your theory more precise. At the time of writing, the ATLAS Collaboration is working on a new analysis with the most precise measurement ever made of the Higgs mass - 8 years later, armed with much more data to reduce the uncertainty, the mass value is still a very important experimental goal.

The Standard Model, moreover, had survived another test. The inexplicable mass of the W and Z bosons seemed to cast doubt - but this experimental discovery showed the triumph of the Standard Model once more as a robust theoretical framework for most of the known universe.

In 2013, Peter Higgs and François Englert, two prominent theorists who initially came up with the Higgs boson, shared the Nobel Prize in Physics for the discovery. Higgs was only in his 30's when he made the groundbreaking theory in the 1960s. He was in his early 80s when the Higgs was found, and the Nobel was awarded. This was an undertaking that spanned a whole career.

## Final Thoughts

Something immediately needs to be said: there is *so, so, much* that I'm neglecting here - from the theory to the analysis. The story I told was a watered-down, triple-distilled, and double-filtered version that had cut many corners. For example, there were many details missing about Lagrangians, and group theory, and quantum fields, and symmetry-breaking. There were many analysis channels, different decay types, different statistical techniques, that I didn't (and can't!) cover more of. Finding the Higgs with ATLAS was a massive project spanning decades involving thousands of scientists. The initial discovery paper [3] has an author and institution list that spans ... 13 pages.

This is the stuff physicists live for. The fact that we can describe systems this thing called a Lagrangian, and interpret the changes to the Lagrangian - when we apply special constraints based on symmetries - as tangible, *physical*, real-life things. How we represent reality in this construct we call mathematics, and from time to time how the mathematics jumps out of the page to give us something real in return. And how, like a perfect puzzle coming together, predictions are in pristine balance with experiment. These are inherently such beautiful ways of knowing, and such elegant ways that nature has decided to ... just exist.

## References & Further Reading

1. [https://en.wikipedia.org/wiki/UA1_experiment](https://en.wikipedia.org/wiki/UA1_experiment)
2. [ATLAS Fact Sheet, 2011](https://cds.cern.ch/record/1457044/files/ATLAS%20fact%20sheet.pdf)
3. [ATLAS Collaboration. *Observation of a new particle in the search for the Standard Model Higgs boson with the ATLAS detector at the LHC*. Physics Letters B, Vol. 716, No. 1, pp. 1-29. 2012.](https://www.sciencedirect.com/science/article/pii/S037026931200857X#fg0080)
4. [https://en.wikipedia.org/wiki/Higgs_boson](https://en.wikipedia.org/wiki/Higgs_boson)
