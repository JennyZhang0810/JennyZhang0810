# UAIV-Foundry

UAIV-Foundry is a low-altitude multimodal data production system for building, auditing, releasing, and benchmarking UAIV-style datasets.

It is not only an awesome list, and it is not a replacement for annotation tools. It combines:

```text
Knowledge Layer
  -> curated resources for datasets, annotation platforms, data quality, synthetic data, and remote sensing VLMs

Data Factory Layer
  -> manifests, batch assignment, Golden Dataset, Labeler import records, annotation export intake, QA, dashboard

Release & Benchmark Layer
  -> dataset cards, release readiness checks, public-package checks, benchmark request protocols, failure-to-data iteration
```

In the UAIV ecosystem:

- `UAIV-Real` is the dataset/product.
- `UAIV-Labeler` is the human annotation platform.
- `UAIV-Foundry` is the production line, QA system, dashboard, release checker, resource index, and benchmark protocol around the dataset.

## Why This Exists

Low-altitude data construction is not just image collection or manual annotation. A publishable dataset also needs:

- clear dataset scope and exclusion decisions;
- reproducible manifests and import records;
- task and worker assignment;
- Golden Dataset calibration;
- annotation export preflight;
- QA gates and rework records;
- dataset cards generated from real statistics;
- release blockers and license/public-link tracking;
- benchmark requests aligned with the released version.

UAIV-Foundry makes these steps explicit, auditable, and reusable.

## Current Status

Current focus: **first-public city governance data package for UAIV-Real**.

| Item | Status |
| --- | --- |
| Cleaned first-public scope | 4,796 images / 5,019 total files |
| Golden Dataset | 96 images generated, waiting for human annotation |
| Labeler import records | Full package and 12 worker-group packages generated |
| Annotation launch readiness | PASS |
| Release package self-check | pre-annotation materials PASS; public release PENDING |
| Public release | blocked by reviewed annotations, final QA, license decision, and public links |
| Benchmark | dry-run request JSONL generated; real benchmark waits for reviewed annotations |

Daily Chinese entry points:

- `/data5/zhangjiening/Data_Construction/UAIV-Foundry/文档入口.md`
- `/data5/zhangjiening/Data_Construction/UAIV-Foundry/近一周进度速读_20260608.md`
- `/data5/zhangjiening/Data_Construction/UAIV-Foundry/中文文档地图.md`
- `/data5/zhangjiening/Data_Construction/UAIV-Foundry/当前状态与下一步.md`

## Repository Map

| Area | Path | Purpose |
| --- | --- | --- |
| Knowledge layer | `awesome/` | Curated external resources for low-altitude datasets, annotation tools, synthetic data, data quality, and remote sensing VLMs |
| Dataset cards | `datasets/` | UAIV-Real dataset cards, first-public manifest builders, and generated card drafts |
| Annotation platforms | `platforms/` | UAIV-Labeler, CVAT, Label Studio, and annotation-platform comparison notes |
| Data generation | `generation/` | Data augmentation and synthetic-data recipes |
| Quality checks | `evaluation/` | Dataset and image quality check templates |
| Production pipelines | `pipelines/` | Data production dry-runs, launch readiness checks, first-public status refresh |
| Annotation QA | `qa/` | Export preflight, annotation QA, rework plans, quality scores, Golden QA template |
| Dashboards | `dashboard/` | Project dashboards, profile dashboards, and trend snapshots |
| Benchmark runner | `benchmark_runner/` | Adapter protocol, metric specs, request JSONL generation, dry-run reports |
| Baseline benchmarks | `benchmarks/` | Reproducible baseline templates for common UAV tasks |
| Docs and release | `docs/` | Planning notes, logs, release checks, project page, outreach materials |

## Knowledge Layer

The awesome layer is a maintained knowledge base, not a loose bookmark list.

Seed sources currently tracked:

- [HumanSignal/awesome-data-labeling](https://github.com/HumanSignal/awesome-data-labeling)
- [wasiahmad/Awesome-LLM-Synthetic-Data](https://github.com/wasiahmad/Awesome-LLM-Synthetic-Data)
- [qiangsun89/UAV-datasets](https://github.com/qiangsun89/UAV-datasets)
- [satellite-image-deep-learning/datasets](https://github.com/satellite-image-deep-learning/datasets)
- [VisDrone/Awesome-VisDrone](https://github.com/VisDrone/Awesome-VisDrone)

Key files:

- `awesome/README.md`
- `awesome/资源条目整理规范.md`
- `awesome/资源库持续更新机制.md`
- `awesome/awesome-annotation-platforms.md`
- `awesome/awesome-low-altitude-datasets.md`
- `awesome/awesome-data-quality.md`
- `awesome/awesome-synthetic-data.md`
- `awesome/awesome-remote-vlm.md`

Each high-quality resource entry should eventually include paper/code/dataset/project-page/documentation links, license/access notes, task, modality, annotation type, scale, and UAIV relevance.

## First-Public City Governance Package

Important files:

| Purpose | Path |
| --- | --- |
| Full manifest | `/data5/zhangjiening/Data_Construction/UAIV-Real/manifests/first_public_city_governance/first_public_city_governance_manifest.csv` |
| Full Labeler import records | `/data5/zhangjiening/Data_Construction/UAIV-Real/manifests/first_public_city_governance/first_public_city_governance_labeler_import_records.json` |
| Golden import records | `/data5/zhangjiening/Data_Construction/UAIV-Real/manifests/first_public_city_governance/golden_subset_labeler_import_records.json` |
| Worker cards | `/data5/zhangjiening/Data_Construction/UAIV-Real/manifests/first_public_city_governance/首发城市治理_标注员任务卡索引.md` |
| Worker import packages | `/data5/zhangjiening/Data_Construction/UAIV-Real/manifests/first_public_city_governance/首发城市治理_分组导入包索引.md` |
| Annotation launch panel | `/data5/zhangjiening/Data_Construction/UAIV-Real/manifests/first_public_city_governance/首发城市治理_标注启动作战面板.md` |
| Export delivery spec | `/data5/zhangjiening/Data_Construction/UAIV-Real/manifests/first_public_city_governance/首发城市治理_标注导出交付规范.md` |
| Golden QA template | `qa/Golden导出后QA执行模板.md` |

## Validation Logic

Foundry's value should be proven with evidence, not slogans.

The validation framework tracks:

- quality evidence: QA errors, warnings, affected image rate, taxonomy issues;
- efficiency evidence: time saved in import generation, batch assignment, export preflight, rework localization;
- reproducibility evidence: manifest/import/card/dashboard/release consistency;
- research evidence: benchmark request coverage and failure-to-data iteration.

Detailed framework:

`docs/规划与说明/UAIV-Foundry价值证明与验证框架_20260609.md`

## Common Commands

Refresh first-public status:

```bash
python pipelines/refresh_first_public_status.py
```

Check annotation launch readiness:

```bash
python pipelines/check_annotation_launch_readiness.py
```

Check release package:

```bash
python docs/release/check_release_package.py
```

Check static project page:

```bash
python docs/site/check_site_readiness.py
```

Check a Labeler export package after Golden/full annotation:

```bash
python qa/check_labeler_export_package.py \
  --export-dir <EXPORT_DIR> \
  --expected-scope golden
```

## Roadmap

- [x] Build repository structure and execution tracker.
- [x] Create initial awesome resource lists.
- [x] Add structured curation rules and continuous-update workflow for resources.
- [x] Build first-public city governance manifest and Labeler import records.
- [x] Generate Golden Dataset and 12 worker-group cards/import packages.
- [x] Add annotation launch readiness checks.
- [x] Add Labeler export preflight template.
- [x] Add QA, dashboard, dataset-card, release-check, and benchmark dry-run components.
- [ ] Run Golden Dataset annotation and QA after human export.
- [ ] Run full annotation QA and rework closure.
- [ ] Finalize dataset card, license, public links, and release package.
- [ ] Run real benchmark after reviewed annotations exist.

## Start Here

- 中文入口：`文档入口.md`
- 近一周速读：`近一周进度速读_20260608.md`
- 中文文档地图：`中文文档地图.md`
- 当前状态：`当前状态与下一步.md`
- 价值证明框架：`docs/规划与说明/UAIV-Foundry价值证明与验证框架_20260609.md`
- 接下来任务清单：`docs/规划与说明/接下来可执行任务清单_20260609.md`
- Main logs:
  - `docs/logs/主线A_数据平台工作日志.md`
  - `docs/logs/主线B_Foundry工作日志.md`

## License

Code and documentation in this repository are released under the MIT License unless otherwise noted. External resources keep their original licenses and terms. Dataset release terms for UAIV-Real must be confirmed before public distribution.
