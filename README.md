<p align="center">
  <img src="https://raw.githubusercontent.com/smorchj/smorchj/refs/heads/main/assets/banner.svg" alt="Sander Mørch-Jensen — Lead Technical Artist at Attensi AS" width="100%" />
</p>

> 9 years in the games industry. Currently spearheading the **full automation of 3D art pipelines** at [Attensi](https://attensi.com) Combining Reallusion Character Creator 4 with the in-house character creator I designed, so that one click turns a client brief into a game-ready GLB. On the side I do experiments like the MetaHuman pipeline below.

---

## What I'm Building

### Reallusion CC4 → GLB Pipeline at Attensi
> **Unity · C# · Python · Reallusion CC4 · Claude Code**

This is my day job. Automating the full path from **Reallusion Character Creator 4** out to game-ready GLBs, plugged directly into the in-house character creator and Unity tooling I designed in the years before generative AI. The combined pipeline is what makes it viable for a small team to deliver customized characters reliably at a large scale to phones, tablets and computers of varying specs, all around the world.


---

### MetaHuman → GLB
> **Unreal Engine 5.6 · Blender 5.0 · Python · three.js · Claude Haiku**

A weekend side project. Takes a MetaHuman out of Unreal and lands it in a browser as a Draco-compressed GLB with a three.js viewer, through a four-stage deterministic pipeline. Tested running in Safari on iPhone X.

<p align="center">
  <a href="https://smorchj.github.io/metahuman-to-glb/">
    <img src="https://raw.githubusercontent.com/smorchj/smorchj/refs/heads/main/assets/metahuman-ada.png" alt="Ada — MetaHuman rendered in the three.js gallery" width="70%" />
  </a>
</p>

<p align="center">
  <a href="https://smorchj.github.io/metahuman-to-glb/">
    <img src="https://img.shields.io/badge/LIVE%20DEMO-metahuman--to--glb-06B6D4?style=for-the-badge&labelColor=0a0420&logo=github&logoColor=white" alt="live demo" />
  </a>
  &nbsp;
  <a href="https://github.com/smorchj/metahuman-to-glb">
    <img src="https://img.shields.io/badge/SOURCE-metahuman--to--glb-A855F7?style=for-the-badge&labelColor=0a0420&logo=github&logoColor=white" alt="source" />
  </a>
</p>

Runs per-stage on Claude Haiku — each stage boundary keeps context small enough that a weak model can execute. MIT-licensed and **open to contributors**; see the [issue tracker](https://github.com/smorchj/metahuman-to-glb/issues) for what's unfinished.

I also built an animated walkthrough of the context-layer model the pipeline uses: it visualises how Opus authors each stage's contract, how Haiku walks the manifest one stage at a time, and how the five context layers (orientation → routing → stage contract → shared references → per-character state) keep each spawned agent's payload small enough that cheap models finish reliably.

<p align="center">
  <a href="https://smorchj.github.io/metahuman-to-glb/icm-agent-flow.html">
    <img src="https://img.shields.io/badge/AGENT%20FLOW%20ANIMATION-watch%20the%20context%20layers%20route-C084FC?style=for-the-badge&labelColor=0a0420" alt="agent flow animation" />
  </a>
</p>

---

### RealTalk: LLMs in Games for Freeform Dialog
> **LLMs · Unity · Game Dialog Systems**

I built the initial product demo for the demo that became RealTalk, integrating LLMs into games to give players genuinely freeform dialog. It became a main part of Attensi's marketing and has since grown into a product selling to big companies. I handed my initial demo to another team that made it into the industry-leading product it is today. I'm proud of both halves of that: proving the idea well enough that the company committed to it, and handing it off cleanly so a specialized team could take it further than I would have alone.

---

### The Character Creator: Automating 3D Pipelines Before Generative AI
> **Unity · C# · Custom Editor Tools · Animation Rigging**

Earlier in my career, 3D character delivery was labour-intensive. Every client project meant grinding through the same work by hand. I therefore made an industry-leading character creator for Unity that automated the bulk of that pipeline and shipped game characters to some of the largest companies in the world. I was in charge of all the logic, architecture and both 3D technical development and 3D asset production (with help on parts of the tool implementation). It predates current generative AI, though I used narrow AI for small pieces even back then. It's the system that taught me what a world-class character creator actually needs when it has to run well on mobile and web, not just look good in a render.

The reviews for the character creator have been nothing short of amazing. It shipped as a core part of Attensi's Creator toolkit and is genuinely fun to use, which is something customers bring up on their own. Getting a 3D production tool to land as "fun" instead of "tolerable" is something greater engineers and designers have failed on before, and it's one of the things I'm most proud of being able to accomplish.

What has changed now is the cost floor. Generative AI has made entire classes of pipelines viable that simply weren't worth building before. My focus has now shifted and my eye is tuned at how I can use AI to reshape the industry.

---

## How I Work

I am not a formally educated software engineer, I'm a technical artist who learned to code because the problems in front of me needed solving. 9 years of shipping games taught me how to set up pipelines that can deliver effectively and consistently in large scale productions.

What that means in practice:

- I know my way around C#, but I am not a code reviewer in charge of core and rather specialize on using tools and scripting to build production pipelines.
- I've been using LLMs, diffusion models, and 3D generators since the early days, in pipelines that make real money, not demos.
- I have great intuition for how to deliver successful large scale 3D production pipelines.

---

## Tech I Use Daily

**Production**

![Unity](https://img.shields.io/badge/Unity-0a0420?style=for-the-badge&logo=unity&logoColor=ffffff&labelColor=0a0420)
![C#](https://img.shields.io/badge/C%23-A855F7?style=for-the-badge&logo=csharp&logoColor=ffffff&labelColor=0a0420)
![Python](https://img.shields.io/badge/Python-06B6D4?style=for-the-badge&logo=python&logoColor=ffffff&labelColor=0a0420)
![Blender](https://img.shields.io/badge/Blender-E879F9?style=for-the-badge&logo=blender&logoColor=ffffff&labelColor=0a0420)
![TypeScript](https://img.shields.io/badge/TypeScript-06B6D4?style=for-the-badge&logo=typescript&logoColor=ffffff&labelColor=0a0420)
![Svelte](https://img.shields.io/badge/Svelte-A855F7?style=for-the-badge&logo=svelte&logoColor=ffffff&labelColor=0a0420)

**Generative AI Stack**

![Claude](https://img.shields.io/badge/Claude%20Code-A855F7?style=for-the-badge&logo=anthropic&logoColor=ffffff&labelColor=0a0420)
![Meshy](https://img.shields.io/badge/Meshy-06B6D4?style=for-the-badge&logoColor=ffffff&labelColor=0a0420)
![Stable Diffusion](https://img.shields.io/badge/Stable%20Diffusion-E879F9?style=for-the-badge&logoColor=ffffff&labelColor=0a0420)
![Wan 2.2](https://img.shields.io/badge/Wan%202.2-06B6D4?style=for-the-badge&logoColor=ffffff&labelColor=0a0420)

---

<a name="klonode"></a>

### Footnote: [Klonode](https://github.com/smorchj/klonode) — AI-driven experiment in context routing
> TypeScript · Svelte · Node.js · Claude Code · ICM

Small experiment, not a main project. Klonode auto-generates per-folder `CONTEXT.md` routing for a git repo so AI coding assistants load only the context they actually need. The codebase is itself mostly AI-written; I'm running it as an open playground for agentic workflows. **AI contributors especially welcome** — pick up an issue and ship.

<a href="https://github.com/smorchj/klonode">
  <img src="https://img.shields.io/badge/SOURCE-klonode-A855F7?style=for-the-badge&labelColor=0a0420&logo=github&logoColor=white" alt="klonode" />
</a>

---

<p align="center">
  <img src="https://raw.githubusercontent.com/smorchj/smorchj/refs/heads/main/assets/footer.svg" alt="Takk for meg" width="100%" />
</p>
