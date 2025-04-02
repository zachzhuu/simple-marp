---
marp: true
theme: academic
paginate: true
math: katex
---

<!-- _class: lead -->

## Language-Based Scene Understanding for Mobile Robot

#### ROAS6800H Seminar 

<br>

**Yiming ZHU, MPhil's Student**
ROAS, Systen Hub
2025/04/01

---

<!-- _header: Contents -->

1. Background
2. **SceneScript**: Reconstructing Scenes With An Autoregressive Structured Language Model
  _What it is, how to train, experiments, why we need?_
1. Application

---

<!-- _header: Background -->

<br/>

![w:1200 center](./images/bg.jpg)

(a) Robust Odometry<sup>1</sup>&emsp;(b) Complex Scenes<sup>2</sup>&emsp;(c) Rich Annotations<sup>3</sup>

> 1: Fast-lio https://ieeexplore.ieee.org/abstract/document/9372856/
> 2: Habitat3.0 https://arxiv.org/abs/2310.13724
> 3: VLA-3D https://arxiv.org/abs/2411.03540

---

<!-- _header: Background -->

- Mainstream methods<sup>1</sup> use scene graph to represent a scene.
- Our work DualMap<sup>2</sup> aims at real-time language navigation.

![w:1200 center](./images/methods.jpg)

> 1: HOV-SG https://arxiv.org/abs/2403.17846
> 2: under review

---

<!-- _header: What is SceneScript? -->

[<u>SceneScript</u>](https://www.projectaria.com/scenescript/) (Meta Reality Labs, ECCV24') is a novel method of **end-to-end** representing scenes using **language**.

<div style="display: flex; justify-content: center; align-items: center; gap: 50px;">
  <video controls src="./images/what.mp4" width="800" height="480" title="Example Video"></video>
  <img src="./images/quest3.jpg" alt="LLM Image" width="300" height="480">
</div>

---

<!-- _header: How is SceneScript trained? -->

Similar to next token prediction in LLMs.

![w:900 center](./images/pipeline.jpg)

---

<!-- _header: How is SceneScript trained? -->

- 3D scene data is not as accessible as web texts for LLM training.
- Synthetic dataset [Aria Synthetic Environments](https://www.projectaria.com/datasets/ase/) with 100K scenes.

![w:900 center](./images/aria.jpg)

---

<!-- _header: Experimental Results -->

The authors tested the performance of SceneScripts on layout estimation & object detection.

![w:900 center](./images/ex.jpg)

---

<!-- _header: Why SceneScript? -->

Low memory, extensibility and integration with language models.

![w:1100 center](./images/why.jpg)

---

<!-- _header: Application -->

[SpatialLM](https://manycore-research.github.io/SpatialLM/) uses the pointcloud encoder of SceneScript. It validates the SceneScript's compatibility with LLM.

![w:1000 center](./images/spatiallm.png)


---

<!-- _header: Application -->

- Spatia"lLM" means Large Language Model, which is **over-claimed**.
- But it inspires us about future directions.

![w:1000 center](./images/genuine.jpg)

---

<!-- _header: Block Test -->

This is a test for blocks.

<div class="block">
  <div class="title">Key Point</div>
  <p><strong>The next generation of robots</strong> will need to build <strong>metric-semantic</strong> representations of environments, enriched with <strong>inter-object relations</strong> and <strong>human-in-the-loop</strong> capabilities.</p>
</div>

They looks all set.

---

<!-- _class: lead -->
## Thank you!

> \* Slides made with [Marp](https://github.com/marp-team/marp) and [kaisugi](https://github.com/kaisugi/marp-theme-academic).