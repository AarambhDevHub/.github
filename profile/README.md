<div align="center">

```
 █████╗  █████╗ ██████╗  █████╗ ███╗   ███╗██████╗ ██╗  ██╗
██╔══██╗██╔══██╗██╔══██╗██╔══██╗████╗ ████║██╔══██╗██║  ██║
███████║███████║██████╔╝███████║██╔████╔██║██████╔╝███████║
██╔══██║██╔══██║██╔══██╗██╔══██║██║╚██╔╝██║██╔══██╗██╔══██║
██║  ██║██║  ██║██║  ██║██║  ██║██║ ╚═╝ ██║██████╔╝██║  ██║
╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝╚═════╝ ╚═╝  ╚═╝
```

### **Start Building. Keep Building.**

High-performance web frameworks, systems tools, and developer education — in **Rust** and **Go**.

<img src="https://img.shields.io/badge/Rust-1.75+-orange?style=for-the-badge&logo=rust&logoColor=white"/>
<img src="https://img.shields.io/badge/Go-1.22+-00ADD8?style=for-the-badge&logo=go&logoColor=white"/>
<img src="https://img.shields.io/badge/open_source-❤️-red?style=for-the-badge"/>

[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@aarambhdevhub)
[![Discord](https://img.shields.io/badge/Discord-Join-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/invite/HDth6PfCnp)
[![Sponsor](https://img.shields.io/badge/Sponsor-GitHub-ea4aaa?style=for-the-badge&logo=github-sponsors)](https://github.com/sponsors/aarambh-darshan)

</div>

---

## ⚡ Flagship Frameworks

Two frameworks. Two languages. One philosophy: **zero compromise on performance.**

<table>
<tr>
<td width="50%">

### [Ajaya (अजय)](https://github.com/AarambhDevHub/ajaya) — Rust

> *"The Unconquerable Rust Web Framework"*

Built on **Tokio + Hyper 1.x**. Zero-allocation hot path. Beats Axum on `ab`, 2× more consistent than Actix on latency.

```
wrk:  291,759 req/sec  @  363µs avg
ab:    27,834 req/sec  @    7ms max
stdev:    369µs  (vs Actix 802µs)
```

![Version](https://img.shields.io/badge/v0.1.6-orange?style=flat-square)
![License](https://img.shields.io/badge/MIT%20%2B%20Apache%202.0-blue?style=flat-square)

</td>
<td width="50%">

### [Rudra (रुद्र)](https://github.com/AarambhDevHub/rudra) — Go

> *"Fierce. Fast. Fearless."*

Built on **net/http + custom radix tree**. Beats Fiber on static routes. **2× faster than Gin and Echo** on parameterized routes. Phase 0 — zero optimizations yet.

```
wrk static:  206,686 req/sec  @  688µs avg
wrk params:  189,005 req/sec  @  708µs avg
vs Fiber:    +2.4%  vs Gin: +46%  vs Echo: +53%
```

![Version](https://img.shields.io/badge/v0.0.9-brightgreen?style=flat-square)
![Phase](https://img.shields.io/badge/phase_0-complete-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/MIT%20%2B%20Apache%202.0-blue?style=flat-square)

</td>
</tr>
</table>

> Both frameworks benchmarked on the same hardware: Intel Core i3-1115G4, 8GB RAM, Pop OS.
> `wrk -t4 -c100 -d10s` — identical test conditions, no tuning applied.

---

## 🛠️ Developer Tools

<table>
<tr>
<td width="50%">

### [typebridge](https://github.com/AarambhDevHub/typebridge)

Rust proc macro SDK that generates **TypeScript, Python, Go, Swift, Kotlin, Zod, GraphQL SDL, and JSON Schema** from annotated Rust structs and enums. One annotation, 8 languages.

```rust
#[typebridge(typescript, python, go, zod)]
pub struct User {
    pub id: Uuid,
    pub email: String,
    pub role: UserRole,
}
```

![Crates](https://img.shields.io/badge/crates.io-published-orange?style=flat-square)
![Workspace](https://img.shields.io/badge/14+_crates-workspace-blue?style=flat-square)

</td>
<td width="50%">

### [Spanda (स्पन्द)](https://github.com/AarambhDevHub/spanda)

Production Rust animation library. 38+ easing functions, spring physics, GPU batch animation via WGSL compute shaders, SVG path parsing, scroll-linked animations, FLIP transitions, color interpolation in Oklch and CIE L\*a\*b\*. Bevy integration. `no_std` support.

![Crates](https://img.shields.io/badge/crates.io-v0.9.1-orange?style=flat-square)
![Features](https://img.shields.io/badge/GPU%20%7C%20Bevy%20%7C%20no__std-blue?style=flat-square)

</td>
</tr>
<tr>
<td width="50%">

### [Vega (वेग)](https://github.com/aarambh-darshan/vega)

Next.js-inspired **file-based routing Rust framework** on top of Axum. Compile-time route codegen via `build.rs` and `syn` — zero runtime overhead, no manual `mod` declarations.

![Stack](https://img.shields.io/badge/Axum%20%7C%20syn%20%7C%20build.rs-blue?style=flat-square)

</td>
<td width="50%"></td>
</tr>
</table>

---

## 🧠 Systems Projects

| Project | Description | Highlight |
|---------|-------------|-----------|
| [mini-database](https://github.com/AarambhDevHub/mini-database) | Graph DB with SQL-like query interface | 138K ops/sec |
| [mini-kafka](https://github.com/AarambhDevHub/mini-kafka) | Distributed message queue in Rust | 347ns latency |
| [mini-redis](https://github.com/AarambhDevHub/mini-redis) | In-memory key-value store | 50K ops/sec |
| [mini-docker-rust](https://github.com/AarambhDevHub/mini-docker-rust) | Container runtime from scratch | Linux namespaces + cgroups |
| [mini-git](https://github.com/AarambhDevHub/mini-git) | Version control system from scratch | Full VCS feature set |
| [multi-cam-face-tracker](https://github.com/AarambhDevHub/multi-cam-face-tracker) | Real-time multi-camera face tracking | Zero-copy frame pipeline |

---

## 📚 Education

### Book — [Aarambh: Your First Real Project](https://buymeacoffee.com/aarambhdevhub)

A no-nonsense guide for Indian CS/Engineering students stuck in tutorial hell. Step-by-step — from zero to a real shipped project.

![Price](https://img.shields.io/badge/₹330%20~%20$3.99-ffdd00?style=flat-square&logo=buy-me-a-coffee&logoColor=black)

### YouTube — [Aarambh Dev Hub](https://youtube.com/@aarambhdevhub)

Deep technical builds — framework internals, proc macros, async Rust, production Go, systems programming. No fluff, full code.

**Series:** Axum Full Course · Rust Animation with Spanda · typebridge Deep Dive

[![Subscribe](https://img.shields.io/badge/Subscribe-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@aarambhdevhub)

### Discord Study Group

Weekly Sunday sessions at **9:30 PM IST** — pick a topic, prepare it, explain it to the group. Rust, Go, systems, architecture.

[![Join](https://img.shields.io/badge/Join%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/invite/HDth6PfCnp)

---

## 🧰 Tech Stack

**Primary:** Rust · Go
**Runtime/Async:** Tokio · net/http · Hyper 1.x
**Frontend:** Leptos 0.7 · Tailwind CSS v4
**Build Tools:** syn · proc-macro2 · build.rs codegen
**Infra:** Linux · Docker · GitHub Actions

---

## 📊 Framework Evolution

This org has been building frameworks since day one. The numbers show the compounding:

| Era | Rust | Go |
|-----|------|----|
| Early | Ignitia — 51,574 req/sec | Blaze — 182,505 req/sec |
| **Now** | **Ajaya — 291,759 req/sec (+466%)** | **Rudra — 206,686 req/sec (+13%)** |

Every framework we've built taught us something. Ajaya and Rudra are what we learned.

---

## 💰 Support the Work

Everything here is open source. If it saves you time or teaches you something:

[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/aarambhdevhub)
[![GitHub Sponsors](https://img.shields.io/badge/GitHub%20Sponsors-ea4aaa?style=for-the-badge&logo=github-sponsors&logoColor=white)](https://github.com/sponsors/aarambh-darshan)
[![Razorpay](https://img.shields.io/badge/Razorpay%20(India)-02042B?style=for-the-badge&logo=razorpay&logoColor=white)](https://razorpay.me/@aarambhdevhub)
[![Fiverr](https://img.shields.io/badge/Hire%20on%20Fiverr-1DBF73?style=for-the-badge&logo=fiverr&logoColor=white)](https://fiverr.com/s/XL1ab4G)

---

<div align="center">

**Aarambh Dev Hub — Start Building. Keep Building.**

*Rust · Go · Systems · Open Source*

</div>
