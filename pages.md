---
marp: true
theme: academic
paginate: true
math: katex
style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
---

<!-- _class: lead -->

## Language-Based Scene Understanding for Mobile Robot

#### UCMP6050 Assignment 5

<br>

**Yiming ZHU, MPhil's Student**
ROAS, Systen Hub
2025/04/14

---

<!-- _header: Overview and Objectives -->

How can we build a robot with human-like abilities in understanding and interacting with its environment?

<div class="columns">
<div>

![h:250 center](./figs/how-human.jpg)

Fig. 1 How humans interact with world<sup>1</sup>.

</div>
<div>

![h:250 center](./figs/triangle.jpg)

Fig. 2 Triangulation strategy<sup>2</sup>.

</div>
</div>

<div class="block">
  <div class="title">Environment Intelligence</div>
  <p>Environmental intelligence refers to human-like, holistic 3D scene understanding that integrates <strong>perception, interaction, learning, and reasoning</strong>.
  </p>
</div>

> 1: Doctoral Thesis by Siyuan Huang: [Human-like Holistic 3D Scene Understanding](https://escholarship.org/uc/item/48n146z7)
> 2: [From CAPTCHA to Commonsense: How Brain Can Teach Us About Artificial Intelligence](https://www.frontiersin.org/journals/computational-neuroscience/articles/10.3389/fncom.2020.554097/full)

---

<!-- _header: Research Method -->

DualMap<sup>1</sup> is designed for **semantic mapping** and **language-based navigation**.
- Frontend (open-set detection) + Backend (stability filter and DualMap building)
- Text query $\rightarrow$ CLIP feature $\rightarrow$ find matching object $\rightarrow$ Navigating

![w:950 center](./figs/method.jpg)

> 1: Online Open-Vocabulary Semantic Mapping for Natural Language Navigation in Dynamic Changing Scenes, under review

---

<!-- _header: Research Method -->

Diffusion models have shown strong capabilities in learning data distributions for image generation and 3D reconstruction tasks. 
They have also been applied to robotic manipulation, such as in Diffusion Policy<sup>3</sup>. This raises an question: **Can diffusion models also enhance robotic perception?**

<div class="columns">
<div>

![h:300 center](./figs/diffusion.jpg)

Fig. 1 What are diffusion models<sup>1</sup>?

</div>
<div>

![h:300 center](./figs/uwm.jpg)

Fig. 2 Unified World Model<sup>2</sup>, RSS2025.

</div>
</div>

> 1: [DiffCAD: Weakly-Supervised Probabilistic CAD Model Retrieval and Alignment from an RGB Image](https://dl.acm.org/doi/10.1145/3658236)
> 2: [Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets](https://arxiv.org/abs/2504.02792)
> 3: [3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations](https://arxiv.org/abs/2403.03954)


---

<!-- _header: Progress and Future Plan -->

The last milestone achieved is shown as Fig. 1, simulation building is on track.

<div class="columns">
<div>

![h:200 center](./figs/result.jpg)

Fig. 1 Comparison on ScanNet dataset.

</div>
<div>

![h:200 center](./figs/sim.jpg)

Fig. 2 Simulation env(debugging).

</div>
</div>

| Due Date    |Milestones                                 |
|-------------|---------------------------------------------|
| 2025-04-20  | Fine-tuning RDT-1B to validate diffusion based model.    |
| 2025-04-27  | Finalize "diffusion map" idea.        |
| 2025-05-05  | Habitat-Sim based simulation built.    |
