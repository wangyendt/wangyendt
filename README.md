<div align="center">
  <img
    alt="header"
    src="https://capsule-render.vercel.app/api?type=waving&height=170&section=header&text=Wayne%20%7C%20%E7%8E%8B%E4%B9%9F&fontSize=44&fontAlignY=35&animation=fadeIn&color=0:F7A91F,100:111827&fontColor=ffffff"
  />
</div>

<h1 align="center">Wayne (王也)</h1>

<div align="center">
  <img
    alt="typing"
    src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=24&duration=2800&pause=1000&color=F7A91F&center=true&vCenter=true&repeat=true&width=820&lines=%E7%AE%97%E6%B3%95%E5%B7%A5%E7%A8%8B%E5%B8%88%20%7C%20Algorithm%20Engineer;%E4%B8%93%E6%B3%A8%E7%AE%97%E6%B3%95%E8%90%BD%E5%9C%B0%EF%BC%8C%E4%B9%9F%E5%81%9A%E5%B7%A5%E5%85%B7%E9%93%BE%E4%B8%8E%E4%BA%A7%E5%93%81%E5%8C%96"
  />
</div>

<div align="center">
  <a href="https://wayne-algorithm-lib.readthedocs.io/">
    <img alt="Docs" src="https://img.shields.io/badge/Docs-pywayne-F7A91F?style=flat-square&logo=readthedocs&logoColor=white" />
  </a>
  <a href="http://wangye.xin">
    <img alt="Website" src="https://img.shields.io/badge/Website-wangye.xin-111827?style=flat-square&logo=vercel&logoColor=white" />
  </a>
  <a href="http://cvllm.com">
    <img alt="Website" src="https://img.shields.io/badge/Website-cvllm.com-111827?style=flat-square&logo=vercel&logoColor=white" />
  </a>
  <a href="mailto:wang121ye@hotmail.com">
    <img alt="Email" src="https://img.shields.io/badge/Email-wang121ye%40hotmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" />
  </a>
  <a href="http://leetcode.com/wangyehope">
    <img alt="LeetCode" src="https://img.shields.io/badge/LeetCode-wangyehope-FFA116?style=flat-square&logo=leetcode&logoColor=black" />
  </a>
  <a href="https://github.com/wangyendt">
    <img alt="GitHub" src="https://img.shields.io/badge/GitHub-wangyendt-111827?style=flat-square&logo=github&logoColor=white" />
  </a>
</div>

<div align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img alt="C++" src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
  <img alt="C#" src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white" />
  <img alt="Java" src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white" />
  <img alt="Swift" src="https://img.shields.io/badge/Swift-FA7343?style=flat-square&logo=swift&logoColor=white" />
  <img alt="MATLAB" src="https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white" />
</div>

<div align="center">
  <img alt="views" src="https://komarev.com/ghpvc/?username=wangyendt&style=flat-square&color=F7A91F" />
</div>

---

## About

我是一名算法工程师，日常工作和开源项目主要围绕：把算法原型变成可复用的库、命令行工具与可部署的系统组件。

I am an algorithm engineer. I focus on turning algorithm prototypes into reusable libraries/CLIs and deployable system components.

### Focus Areas

* Signal processing / time-series: filtering, peak detection, similarity, spectrograms
* Robotics / vision tooling: calibration, SE(3)/SO(3), tags, visualization utilities
* Developer productivity: automation, cross-device messaging, packaging, docs
* Agent engineering: skills, guardrails, reproducible workflows for coding agents

---

## Selected Projects

| Repo | What it is | Notes |
| --- | --- | --- |
| [`wayne_algorithm_lib`](https://github.com/wangyendt/wayne_algorithm_lib) | `pywayne` toolset for Python & C++ workflows (DSP, CV/robotics utils, automation/integrations). | Docs: https://wayne-algorithm-lib.readthedocs.io/ |
| [`wayne-skills`](https://github.com/wangyendt/wayne-skills) | Production-oriented `SKILL.md` playbooks built around the `pywayne` ecosystem. | Curated, source-aligned, predictable structure |
| [`skillmanager`](https://github.com/wangyendt/skillmanager) | Cross-platform skills manager: install/update skills from official/3rd-party/your repos, with optional Web UI selection. | Based on `openskills` |
| [`ios_tools`](https://github.com/wangyendt/ios_tools) | Swift Package for Apple ecosystem utilities (OpenAI, Lark/Feishu bots, Aliyun OSS, cross-comm, etc.). | iOS/macOS/watchOS/tvOS |
| [`java_tools`](https://github.com/wangyendt/java_tools) | Java toolset for Lark/Feishu, Aliyun OSS, OpenAI API, and cross-comm Java client. | Multi-module Maven project |
| [`cpp_tools`](https://github.com/wangyendt/cpp_tools) | C++ tools fetch/build helpers (3rd-party libs, build scripts). | Utilities for C++ dev setup |
| [`wekws`](https://github.com/wangyendt/wekws) | Keyword spotting (KWS) related experiments / notes. |  |

---

## Ecosystem Map

```mermaid
flowchart TD
  %% Skill layer
  SM[skillmanager<br/>(@wang121ye/skillmanager)] -->|installs / updates / sync AGENTS.md| WS[wayne-skills<br/>(SKILL.md pack)]

  %% Source-aligned skills
  WS -->|source-aligned playbooks| PY[pywayne<br/>(wayne_algorithm_lib)]

  %% C++ toolchain
  PY -->|bin/gettool<br/>fetch/build/install| CPP[cpp_tools<br/>(C++ 3rd-party/tool scripts)]

  %% Cross-language parity
  PY -->|features| F1[OpenAI / Lark(Feishu) / Aliyun OSS / CrossComm]
  IOS[ios_tools<br/>(Swift Package)] -->|same API areas| F1
  JAVA[java_tools<br/>(Maven multi-modules)] -->|same API areas| F1

  %% Optional: direct usage paths
  WS -. curated selection .->|profiles| SM
```

### How The Pieces Fit

* `skillmanager` 管理 skills 来源（官方/第三方/自研），并通过 `openskills` 安装到 `.claude/skills` 或 `.agent/skills`，同时同步生成/更新 `AGENTS.md`。
* `wayne-skills` 是把 `pywayne` 的源码能力转换成可复用的 `SKILL.md` 工作流（强调 “source-aligned”: skill 路径与模块路径一一对应）。
* `pywayne` 提供 Python 侧的可复用模块与命令行工具，其中 `gettool` 用于从 `cpp_tools` 拉取/稀疏检出第三方 C++ 工具与库，并可选执行 build/install。
* `ios_tools` / `java_tools` 提供与 `pywayne` 中相近的“平台集成能力”在 Swift / Java 生态的实现（OpenAI、飞书、OSS、CrossComm 等），便于跨平台复用同一套业务能力。

---

## Docs

* `pywayne` documentation: https://wayne-algorithm-lib.readthedocs.io/
* If you are using agent skills: check `wayne-skills` and `skillmanager`

---

## Common Commands

### skillmanager (install/manage skills)

```bash
# Install (global)
npm i -g @wang121ye/skillmanager@latest

# Install skills (interactive selection by default) + sync AGENTS.md
skillmanager install

# Web UI selection (save a profile)
skillmanager webui --profile laptop
skillmanager install --profile laptop

# Add your own skill source repo (e.g. wayne-skills)
skillmanager source add https://github.com/wangyendt/wayne-skills.git
skillmanager source list

# Update installed skills
skillmanager update

# Show config paths (sources.json, profiles, etc.)
skillmanager paths
```

### pywayne (Python library)

```bash
# Install / upgrade
pip install -U pywayne

# Quick sanity check
python -c "import pywayne; print('pywayne OK')"
```

### gettool (C++ tools fetcher, backed by cpp_tools)

```bash
# List available tools
gettool -l

# Fetch to default path (based on name_to_path_map.yaml)
gettool opencv
gettool eigen

# Fetch + build (if buildable)
gettool apriltag_detection -b

# Fetch + install (if installable)
gettool pcl -i

# Repo URL management
gettool --get-url
gettool --set-url <URL>
gettool --reset-url
```

### cpp_tools (direct usage)

```bash
git clone https://github.com/wangyendt/cpp_tools.git
```

### java_tools (Maven)

```bash
git clone https://github.com/wangyendt/java_tools.git
cd java_tools
mvn clean install

# Run a module (example: aliyun_oss)
cd aliyun_oss
mvn exec:java
```

### ios_tools (Swift Package Manager)

Add to your `Package.swift`:

```swift
.package(url: "https://github.com/wangyendt/ios_tools.git", branch: "main")
```

Local run demos (repo root):

```bash
swift run OpenAIDemo
swift run LarkBotDemo
swift run LarkCustomBotDemo
swift run AliyunOSSDemo
swift run CrossCommDemo listen
```

---

## Stats

<div align="center">
  <img height="180em" alt="stats" src="https://github-readme-stats.vercel.app/api?username=wangyendt&show_icons=true&theme=radical&include_all_commits=true&count_private=true"/>
  <img height="180em" alt="langs" src="https://github-readme-stats.vercel.app/api/top-langs/?username=wangyendt&layout=compact&langs_count=8&theme=radical"/>
</div>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wangyendt/wangyendt/master/profile-3d-contrib/profile-night-rainbow.svg"/>
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/wangyendt/wangyendt/master/profile-3d-contrib/profile-green-animate.svg"/>
    <img width="100%" alt="3d contributions" src="https://raw.githubusercontent.com/wangyendt/wangyendt/master/profile-3d-contrib/profile-night-rainbow.svg"/>
  </picture>
</p>

---

## Contact

* Email: `wang121ye@hotmail.com`, `y-w22@mails.tsinghua.edu.cn`
* Website: http://wangye.xin, http://cvllm.com
* LeetCode: https://leetcode.com/wangyehope
* GitHub: https://github.com/wangyendt


