<div align="center">

# Vighnesh Patidar

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1000&color=7AA2F7&center=true&vCenter=true&width=650&lines=Embedded+Systems+%7C+RTOS+Internals;Distributed+Systems+%7C+Swarm+Robotics;RISC-V+%7C+Bare-Metal+Firmware;C%2B%2B17+%7C+Network+Protocols)](https://git.io/typing-svg)

</div>

Final-year Civil Engineering undergrad at IIT Kanpur (Class of 2026) who spends most of his time several layers below civil engineering — in firmware, distributed systems, and robotics runtimes.

Past stints at **DRDO**, **C3iHub IIT Kanpur**, **NYU**, and **Nambikkai Rehabilitation Devices** (as Chief Software/Firmware Engineer). I like building things from first principles — parsers, schedulers, transports, allocators — rather than reaching for a library.

---

## What I've been building

**[mith-atomas](https://github.com/Vighnesh-Patidar/mith-atomas)**
Decentralized swarm robotics orchestration runtime in C++17 — hybrid ECS architecture, async DAG-based system scheduler, transport-agnostic comms with Ed25519 identity and TOFU, ML-ready action interface.

**[myth-eye-cal](https://github.com/Vighnesh-Patidar/myth-eye-cal)**
Distributed pose reconstruction across a self-organizing phone network. Any phone with line of sight shares keypoints; every phone renders the fused skeleton. No server, no fixed infrastructure. Built on top of mith-atomas.

**[The-Notorious-E.S.P](https://github.com/Vighnesh-Patidar/The-Notorious-E.S.P)**
A bare-metal Wi-Fi packet sniffer for the ESP8266, built entirely from scratch — static slab allocator, lock-free ring buffer, hand-rolled 802.11/IPv4/TCP/UDP parser, and a bitmask-based filter engine. Validated on hardware.

**[run-V.M.C.](https://github.com/Vighnesh-Patidar/run-V.M.C.)**
A RISC-V RV32I virtual machine in C++ — custom memory map, memory-mapped UART, hand-rolled instruction decoder, no emulation libraries.

**[CS315_Redis_From_Scratch](https://github.com/Vighnesh-Patidar/CS315_Redis_From_Scratch)**
A from-scratch C++ implementation of Redis, built as a group project for CS315 at IIT Kanpur.

---

## Currently

- Contributing to **Zephyr RTOS** (syscall stack usage reporting)
- Writing a [Medium series](https://medium.com/@wishu.pradeep) walking through how computers and processors actually work, from binary arithmetic up
- Planning a Bhopal → Bangalore break-in run on a Royal Enfield Super Meteor 650

---

## Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Vighnesh-Patidar&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" width="49%" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vighnesh-Patidar&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" width="35%" />

<img src="https://streak-stats.demolab.com/?user=Vighnesh-Patidar&theme=tokyonight&hide_border=true" width="65%" />

</div>

> The language card above is fed live by GitHub's own byte-count-per-language API, scoped to your non-fork repos — no setup needed, it just works the moment this is your profile README.

### Lines of code

GitHub doesn't expose total lines authored through its API — every "lines of code" badge that actually works pulls it from a one-time GitHub Action setup (it clones your repos and diffs them), not a live query param. Worth doing properly rather than faking it:

1. Generate a **classic PAT** with `repo` scope → Settings → Developer settings → Personal access tokens.
2. In your `Vighnesh-Patidar/Vighnesh-Patidar` repo, add it as a secret named `METRICS_TOKEN`.
3. Add `.github/workflows/metrics.yml`:

```yaml
name: Lines of code metrics
on:
  schedule:
    - cron: '0 0 * * 0'   # weekly refresh
  workflow_dispatch:

jobs:
  lines-of-code:
    runs-on: ubuntu-latest
    steps:
      - uses: lowlighter/metrics@latest
        with:
          filename: metrics.lines.svg
          token: ${{ secrets.METRICS_TOKEN }}
          base: ""
          plugin_lines: yes
          plugin_lines_repositories_limit: 20
          plugin_lines_history_limit: 50
```

4. Run it once from the Actions tab, then reference the committed SVG in this README:

```markdown
![Lines of code](./metrics.lines.svg)
```

It commits `metrics.lines.svg` straight into the repo and refreshes weekly — accurate, not a guess.

---

## Stack

![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white)
![RISC-V](https://img.shields.io/badge/RISC--V-283272?style=for-the-badge&logo=riscv&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Zephyr](https://img.shields.io/badge/Zephyr%20RTOS-686E75?style=for-the-badge&logo=zephyrproject&logoColor=white)

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vighnesh-patidar-1aa61a258/)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/VighneshPatidar)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@wishu.pradeep)

</div>
