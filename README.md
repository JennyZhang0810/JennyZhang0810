<div align="center">

# Jenny Zhang / Zhang Jiening

**PhD Student @ UESTC · Computer Vision · Remote Sensing · Data-centric AI**

> Data is not just fuel. It defines what a model can see, learn, and generalize.

Low-altitude UAV Datasets · Data Production Systems · Structure-aware Synthesis · Low-shot Detection · Benchmark Construction

[![Email](https://img.shields.io/badge/Email-jennyzhang@std.uestc.edu.cn-333?style=flat-square&logo=gmail&logoColor=white)](mailto:jennyzhang@std.uestc.edu.cn)
[![GitHub](https://img.shields.io/badge/GitHub-JennyZhang0810-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/JennyZhang0810)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Jenny%20Zhang-4285F4?style=flat-square&logo=google-scholar&logoColor=white)](https://scholar.google.com.hk/citations?user=ONaB5qUAAAAJ)


</div>

---

## About

I am a Master-PhD combined program student at the [School of Computer Science and Engineering](https://www.scse.uestc.edu.cn/), [University of Electronic Science and Technology of China](https://www.uestc.edu.cn/), and a member of [Center for Future Media](https://cfm.uestc.edu.cn/index), UESTC.

My research focuses on **data-centric computer vision** for remote sensing and low-altitude UAV perception. I study how data is generated, labeled, evaluated, released, and reused, with current interests in low-altitude multimodal datasets, data production operating systems, structure-aware synthetic data, low-shot detection, and benchmark construction.

Advised by [Prof. Wang Guoqing](https://scholar.google.com.hk/citations?hl=zh-CN&user=V08v5OEAAAAJ) and [Prof. Yang Yang](https://cfm.uestc.edu.cn/~yangyang/).

**Keywords:** `Data-centric AI` · `Low-altitude UAV Dataset` · `Data Production OS` · `Remote Sensing` · `Synthetic Data` · `Few-shot Detection` · `Metadata-first Labeling` · `Benchmark Construction`

<!-- <p align="center">
  <img src="https://raw.githubusercontent.com/JennyZhang0810/UAIV-Labeler/main/assets/sample_preview.gif" width="70%" alt="UAIV-Labeler Preview">
</p> -->

---

## Recent News

- 🎤 **[2026.06] Invited to give a talk at the 2026 International Conference on UAV Applications and Countermeasures / 2026 Conference on Intelligent Unmanned Systems and Applications**, presenting my work as the only student speaker in the event.
- 🧭 **[2026.06] Prepared the initial [UAIV-Foundry](https://jennyzhang0810.github.io/UAIV-Foundry/) project page**, a data production operating system for low-altitude multimodal datasets. The project is currently in pre-release engineering status.
- 🔥 **[2026.05] Released [UAIV-Labeler](https://jennyzhang0810.github.io/UAIV-Labeler/)**, an open-source semi-automatic labeling platform for low-altitude UAV remote-sensing datasets. Code is available on [GitHub](https://github.com/JennyZhang0810/UAIV-Labeler), with a live demo at [8.137.184.86](http://8.137.184.86/).
- 🔥 **[2026.05] Released the [UAIV Low-Altitude Multimodal Dataset](https://jennyzhang0810.github.io/LowAltitude-Multimodal-Dataset/)**, with code on [GitHub](https://github.com/JennyZhang0810/LowAltitude-Multimodal-Dataset) and data hosted on [ScienceDB](https://www.scidb.cn/detail?dataSetId=203705443be44f7882bb9ddfd7d401da).
- 📑 **[2026.05] [S²-Det](https://github.com/JennyZhang0810/Neurips2026-s2det)**, Structure-Aware Synthesis for Few-Shot Detection, is under review at **NeurIPS 2026**.
- 📄 **[2024] Published underwater image restoration work in Applied Optics**.
- 🏆 **[2025] National Scholarship and FLTRP Cup National English Debate Champion & Best Debater**.

---

## UAIV Low-Altitude Data Ecosystem

**UAIV Low-Altitude Data Ecosystem**  
[![Dataset Project](https://img.shields.io/badge/Dataset-Project%20Page-2f5f8f?style=flat-square)](https://jennyzhang0810.github.io/LowAltitude-Multimodal-Dataset/)
[![Dataset GitHub](https://img.shields.io/badge/Dataset-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/JennyZhang0810/LowAltitude-Multimodal-Dataset)
[![ScienceDB](https://img.shields.io/badge/Dataset-ScienceDB-4b6f44?style=flat-square)](https://www.scidb.cn/detail?dataSetId=203705443be44f7882bb9ddfd7d401da)
[![Labeler](https://img.shields.io/badge/Labeler-Project%20Page-167c80?style=flat-square)](https://jennyzhang0810.github.io/UAIV-Labeler/)
[![Foundry](https://img.shields.io/badge/Foundry-Project%20Page-b87918?style=flat-square)](https://jennyzhang0810.github.io/UAIV-Foundry/)

My current low-altitude data work is organized as a data-centric stack. The goal is not only to publish a dataset or an annotation tool, but to make the whole data lifecycle reproducible:

```text
Data collection -> Data annotation -> QA and release -> Benchmark evaluation -> Data iteration
```

| Layer | Project | Role | Entry Points |
|:--|:--|:--|:--|
| Data Generation | **S²-Det** | Structure-aware synthetic data generation for few-shot remote-sensing object detection; studies how spatial priors and distribution matching affect synthetic data utility. | [Code](https://github.com/JennyZhang0810/Neurips2026-s2det) |
| Dataset Product | **UAIV-Real / UAIV Dataset** | Public-facing low-altitude multimodal UAV dataset for urban/ecological perception, restoration, and benchmark construction. | [Project](https://jennyzhang0810.github.io/LowAltitude-Multimodal-Dataset/) · [GitHub](https://github.com/JennyZhang0810/LowAltitude-Multimodal-Dataset) · [ScienceDB](https://www.scidb.cn/detail?dataSetId=203705443be44f7882bb9ddfd7d401da) |
| Data Annotation | **UAIV-Labeler** | Human-in-the-loop annotation workbench for metadata-aware indexing, model pre-annotation, scene/object/OCR/event/environment labeling, review, and export. | [Project](https://jennyzhang0810.github.io/UAIV-Labeler/) · [GitHub](https://github.com/JennyZhang0810/UAIV-Labeler) · [Live Demo](http://8.137.184.86/) |
| Data Infrastructure | **UAIV-Foundry** | Data production OS that organizes resources, generates manifests, calibrates Golden samples, checks annotation quality, prepares releases, runs benchmark protocols, and turns failures into the next data iteration. | [Project](https://jennyzhang0810.github.io/UAIV-Foundry/) · [GitHub](https://github.com/JennyZhang0810/UAIV-Foundry) |

The goal is to move beyond releasing isolated datasets or tools, and instead build a reproducible data-centric workflow:

```text
UAIV-Real is what we release.
UAIV-Labeler is where data is annotated.
UAIV-Foundry is how we make the process auditable, measurable, and reusable.
```

This stack is designed to turn low-altitude UAV data construction into a reproducible data-centric workflow rather than a one-off dataset release.

---

## Publications / Preprints

- **S²-Det: Structure-Aware Synthesis for Few-Shot Detection**  
  *Under review at NeurIPS 2026.*  
  Studies how explicit spatial structure priors and distribution matching can make synthetic remote-sensing images more useful for few-shot detection.  
  [Code](https://github.com/JennyZhang0810/Neurips2026-s2det)

- **Underwater Image Restoration with Adaptive Color Correction and Dehazing**  
  *Applied Optics, 2024.*  
  Proposes a hybrid restoration framework that combines adaptive color correction and dehazing for underwater image enhancement.  
  [Paper](https://opg.optica.org/ao/abstract.cfm?uri=ao-63-10-2728)

---

## Academic Service and Invited Talks

- **Invited Speaker**, 2026 International Conference on UAV Applications and Countermeasures / 2026 Conference on Intelligent Unmanned Systems and Applications, 2026. Presented my research as the only student speaker in the event.
- **Reviewer**, *CAAI Transactions on Intelligence Technology*, 2026. CAAI flagship journal; CAS Zone 1 Top, JCR Q1, IF 7.3.

---

## Intellectual Property

**Patent**

- A semantic-guided intelligent generation method for visible-light remote-sensing images.

**Software Copyrights**

- Semantic-guided multi-degradation image restoration system V1.0.
- Information-controllable remote-sensing object image simulation software V1.0.
- Intelligent air-combat advantage calculation and multi-aircraft cooperative combat situation analysis software V1.0.
- Worker operation standardization visual detection algorithm software V1.0.

---

## Honors

| Year | Honor | Note |
|:--|:--|:--|
| 2025 | National Scholarship | Awarded during graduate study with a full GPA record |
| 2025 | First-class Academic Scholarship, UESTC | Graduate academic scholarship |
| 2025 | Outstanding Graduate Student, UESTC | University-level academic honor |
| 2025 | Outstanding Graduate Student Cadre, UESTC | University-level service and leadership honor |
| 2024 | Outstanding Graduate, Shandong Province | Provincial graduate honor |
| 2024 | Outstanding Student Cadre, Shandong Province | Provincial service and leadership honor |
| 2024 | Outstanding Undergraduate Thesis, Shandong Province | Provincial thesis honor |
| 2023 | Ranked 1st academically during undergraduate study | Recommended for postgraduate admission to UESTC |

---

## Media and News Coverage

**Personal features**

- UESTC "Holistic Education" youth representative feature: [WeChat article](https://mp.weixin.qq.com/s/u7JlelEkxGUc0SlxUXVZPQ)

**Team and school stories**

- School of Computer Science and Engineering, UESTC news: [SCSE news page](https://www.scse.uestc.edu.cn/info/1009/18228.htm)
- UESTC / team story: [WeChat article](https://mp.weixin.qq.com/s/IMV4qFgPZWVSXwCr3tRiOQ)

---

## Competitions

<details>
<summary><b>Selected competition awards</b></summary>

<br>

| Competition | Award / Rank |
|:--|:--|
| China International College Students' "Internet+" Innovation and Entrepreneurship Competition | National Bronze Award, ranked 1st |
| Shandong University Student Innovation and Entrepreneurship Competition | Provincial Gold Award, highest award, ranked 1st |
| 2025 China International College Students' Innovation Competition, Higher Education Track | Provincial Silver Award, ranked 1st |
| 2nd Sichuan Provincial College Student Career Planning Competition, Graduate Employment Track | Provincial Bronze Award |
| 27th FLTRP Cup National English Debate Competition | National Gold Award & National Best Debater |
| Chinese Collegiate Computing Competition | National Third Prize |
| National University Student Intelligent Car Race | National Second Prize |

</details>

---

## Community

Beyond research, I share learning methods, PhD life, and personal growth content with Chinese student communities, with 30K+ followers across [Xiaohongshu](https://www.xiaohongshu.com/user/profile/5b83ef0e3be32600019bdeba), Zhihu, and [CSDN](https://blog.csdn.net/qq_53826699). I have also hosted offline reading clubs and student talk sessions.

---

## Collaboration

I am open to collaborations on:

- Remote-sensing image generation and synthetic data evaluation.
- Low-altitude UAV dataset construction and annotation systems.
- Data production infrastructure for annotation QA, dataset release, and benchmark iteration.
- Data-centric AI for object detection, segmentation, restoration, and benchmark design.
- Customized annotation workflows for UAV/remote-sensing tasks.

Contact:

- Official: [jennyzhang@std.uestc.edu.cn](mailto:jennyzhang@std.uestc.edu.cn)
- Personal: 870076398@qq.com

---

<details>
<summary><b>GitHub Stats</b></summary>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=JennyZhang0810&theme=default" />
</div>

<br>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=JennyZhang0810&theme=github-light" />
</div>

</details>

---

<p align="center">
  <sub>If you find my work interesting, welcome to follow, star, or collaborate.</sub>
</p>
