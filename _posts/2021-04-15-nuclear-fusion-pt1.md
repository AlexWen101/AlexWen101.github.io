---
layout: post
title: "Bottling the Sun, Part 1"
author: "Alex Wen"
categories: journal
tags: []
image: iter-tokamak-plasma.jpg
---

In 2019, around 85% of global energy demand was met with fossil fuels - coal, oil, and natural gas. Even if we ignore the obvious environmental damage caused by burning off all our fossil fuels, we'll never escape the other issue: they won't last forever! An *Our World in Data* article [1] estimates that our remaining reserves of fossil fuels, when pitted against mid-2010's level demands, will last between 50-100 years. That's not some far-off problem...

Some enticing replacements are already on the table: wind, solar, nuclear, biomass, hydroelectric, and so on. Let's jump into the story of the golden child, nuclear fusion - and see what the excitement's all about.

## Electricity

A lot of the time, making electricity is all about making something spin. Because of how electric and magnetic fields obey certain laws, we know that a spinning magnet, if set up correctly, induces an electric current - which can then flow to cities and power our heaters and electronics.

How can we get magnets to spin? Well, a popular way is to push fast and pressurized fluids like water or air through a turbine, which is just something that spins as fluids move through it. We can raise them up high and let the wind spin them...

<center><img src="{{ site.github.url }}/assets/img/windturbine.jpg" alt="sm" width="350"/></center>

...or dunk them in water and let the river or ocean spin them.

<center><img src="{{ site.github.url }}/assets/img/hydrodam.jpg" alt="sm" width="350"/></center>

Another way is make our own pressurized fluids - we can boil off lots of water, turn it into steam, and force the steam through a turbine. This method has proven to be quite popular, because unlike wind turbines or dams, we can build them almost anywhere.

So the question is, how do we boil off a whole bunch of water?

This is where we can be a bit creative. The most simple way is to burn stuff with chemical reactions - coal, gas, even wood - but these aren't so great, because like I said, they'll eventually run out soon on earth - not to mention their environmental damage in emitting pollution.

Nuclear power is another option. One proved and tested method is the splitting, or fission, of uranium - we take an atom of uranium and hit it with a neutron, which makes the uranium split apart. These fragments are highly energetic, so if we surround them with water, they'll slam into the water and deposit their energy, heating it. Therefore, in practice, most fission reactors consist of rods of solid uranium, sitting in a tank of water.

<center><img src="{{ site.github.url }}/assets/img/reactorcore.jpg" alt="sm" width="400"/></center>

Another nuclear reaction we might consider is the combination of hydrogen atoms. If we get them to collide into each other fast enough, they'll *fuse* into a heavier element, releasing a very fast neutron, carrying a lot of energy. It's much harder because, among other reasons, we need to subject the hydrogen to *very* specific and extreme reaction conditions which are challenging to engineer. This is the same type of nuclear reaction that occurs in the sun, where the enormous pressure from the sun's mass enables the hydrogen to fuse.

## Fusion's Promise

We've already perfected fission reactors - they're all over the world, from Japan to Canada, and are a safe, reliable, and (relatively) clean source of energy. Fusion isn't even commercially possible yet, and for now doesn't exist outside of certain research lab settings.

So why do we even care about fusion, when we already have fission? The short answer is that fusion's just *too* perfect of an energy source to ignore. The benefits of a fusion-powered world would make research costs seem like a pittance by comparison.

### Pollution

A good way to quantify pollution is to measure the amount of greenhouse gases emitted per unit of electric energy (measured in gigawatt-hours) generated.

Burning fossil fuels will emit anywhere from ~500 to ~800 tonnes of greenhouse gases per gigawatt-hour, while nuclear will only emit around 3 tonnes [2]. That's a *couple-hundred-fold* cleaner in terms of emissions.

In perspective, replacing all US fossil fuel-burning power stations with nuclear plants would immediately cut 15% of all US greenhouse gas emissions [3]. That's like eliminating *all* residential *and* commercial greenhouse gas emissions [3], everything from heating buildings to garbage treatment!

### Safety

A similar conclusion can be made for safety. If we factor in the deaths due to pollution, as well as from various accidents, coal and oil kill around 300 times more people per unit of energy generated than nuclear [2]. The cleanest fossil fuel - natural gas - still kills 40 times more people.

Up to this point, everything we've discussed applies to nuclear power *in general*, especially fission. In my opinion, there's already a great case for confidently adopting more widespread fission power.

If you're like my parents, though, no amount of statistics will ever quell the terrifying radioactive elephant in the room:

<center><img src="{{ site.github.url }}/assets/img/chernobyl.jpg"  width="450"/></center>
<center><i>From HBO's "Chernobyl".</i></center>

An uncontrolled fission reaction may release too much energy and melt the surroundings or explode, spreading a slew of radioactive substances. Fission produces, among other things, a certain reaction by-product called caesium-137. This is nasty stuff [4]. It vaporizes, so it's easily spread around the world by the wind and atmosphere. It's water soluble, so it makes its way into oceans and waterways. It bioaccumulates, so it starts concentrating in the food chain, ultimately making its way into humans, often causing cancer.

While fission nuclear disasters are few and rare, and while *statistically* there really is negligible risk of death by nuclear accident, public perception of nuclear power has forever been tarnished by scary disasters like [Chernobyl](https://en.wikipedia.org/wiki/Chernobyl_disaster) and [Fukushima](https://en.wikipedia.org/wiki/Fukushima_Daiichi_nuclear_disaster).

Fusion has *none* of these concerns. Some fusion methods will produce a slightly radioactive by-product called tritium, but (if spilled) tritium emits milder radiation, stays radioactive for shorter, and doesn't bioaccumulate, compared to caesium. More importantly, fusion reactors can *never* melt down or explode. This is because they don't rely on runaway fission reactions that must be controlled - if anything goes wrong, the fusion reaction simply stops (we'll see why later!), the opposite of releasing too much energy.

So *even if* fusion created the same toxic by-products as fission (which it doesn't), it's still definitively safe. Even the most fearful nuclear skeptics can rest assured of fusion's immunity from nuclear disaster.

<center><img src="{{ site.github.url }}/assets/img/death-rates-from-energy-production-per-twh.png"  width="550"/></center>
<center><i>From [2].</i></center>

### Fuel Security

This one's straightforward. As we mentioned earlier - fossil fuels are going to run out in a matter of decades. In contrast, fusion reactions consume an isotope of hydrogen called deuterium (a component of the well-known chemical "heavy water"), which we have an effectively unlimited supply of. Most fusion reactors also consume a metal called lithium. Earth's supply of lithium, assuming all power is generated from fusion, will last around ... 6 million years [5].

### Proliferation

Finally, when we look past the science, we remember that some states use nuclear power as an excuse to enrich uranium for nuclear weapons. This is a real concern with fission - it uses enriched uranium. Enrich it too much (on purpose), and you can fabricate a bomb.

In contrast, fusion power doesn't share any fundamental technologies with creating nuclear weapons; someone can't claim to create nuclear fusion fuel while really trying to make a bomb. If fusion were the norm, it would be easier to identify and control nuclear proliferation.

## Final Thoughts

Fusion is almost perfect - it has everything you could possibly ask for in a energy source. It's clean, it uses readily available fuel, and it's *infallibly* safe. It almost feels like we're cheating, and makes our current sources of energy (like coal) seem ancient and rudimentary in comparison. You almost can't find any complaints! That's why there's so much investment - the rewards are just too great.

But we should really stop daydreaming - after all, we still don't even have fusion power yet. In the next post on this topic, we'll talk about physics, plasmas, and principles, surrounding current attempts at fusion, and why it's so damn hard to achieve!

<center><img src="{{ site.github.url }}/assets/img/fusion-comic.png"  width="550"/></center>

## References & Further Reading

1. [https://ourworldindata.org/how-long-before-we-run-out-of-fossil-fuels](https://ourworldindata.org/how-long-before-we-run-out-of-fossil-fuels)
2. [https://ourworldindata.org/safest-sources-of-energy](https://ourworldindata.org/safest-sources-of-energy)
3. [https://www.epa.gov/ghgemissions/sources-greenhouse-gas-emissions](https://www.epa.gov/ghgemissions/sources-greenhouse-gas-emissions)
4. [https://en.wikipedia.org/wiki/Caesium-137](https://en.wikipedia.org/wiki/Caesium-137)
5. [https://www.iter.org/sci/FusionFuels](https://www.iter.org/sci/FusionFuels)
6. [https://en.wikipedia.org/wiki/Nuclear_fusion](https://en.wikipedia.org/wiki/Nuclear_fusion)
