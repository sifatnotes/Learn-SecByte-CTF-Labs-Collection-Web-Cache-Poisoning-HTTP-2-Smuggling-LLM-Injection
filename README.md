# Learn-SecByte-CTF-Labs-Collection-Web-Cache-Poisoning-HTTP-2-Smuggling-LLM-Injection
A curated collection of hands-on cybersecurity CTF labs covering Web Cache Deception, HTTP/2 Request Smuggling, HTTP/2 Rapid Reset, Host Header Poisoning, HPP, and LLM Output Injection from Learn SecByte.
# Learn SecByte CTF & Cybersecurity Labs Collection

Welcome to the **Learn SecByte CTF & Cybersecurity Labs Collection**. This repository is a dedicated, searchable index of hands-on Web Cache Poisoning & Deception (Web Cache Desynchronization, Cache Entanglement, Cache Key Confusion, HTTP Cache Deception), Protocol & HTTP Smuggling Attacks (HTTP/2 Request Smuggling, HTTP/2 Rapid Reset DoS), HTTP Parameter & Verb Tampering (HTTP Verb Tampering, HTTP Method Override Abuse, HTTP Parameter Fragmentation, HTTP Parameter Pollution, Host Header Poisoning), and AI/LLM Security (LLM Output Injection, Prompt Abuse, Tool Hijacking) labs designed for cybersecurity students, CTF players, application security engineers, cloud architects, bug bounty hunters, and AI safety researchers.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Securing complex web architectures and modern AI-driven platforms requires understanding protocol-level desynchronization, cache key manipulation, and untrusted output execution paths. Hosted on [Learn SecByte](https://learn.secbyte.org/), this advanced web cache desynchronization, HTTP/2 request smuggling, parameter parsing ambiguity, and LLM output injection collection provides practical, hands-on technical training to audit, exploit, and remediate low-level web infrastructure and AI integration vulnerabilities.

From manipulating unkeyed headers to poison web caches, abusing cache key normalizations to trick reverse proxies into storing sensitive user profiles (`HTTP Cache Deception`), and downgrading HTTP/2 frames to launch request smuggling attacks to abusing stream cancellation resets (`HTTP/2 Rapid Reset`), bypassing access controls via HTTP verb tampering and parameter pollution (`HPP`), poisoning host headers for password reset link hijacking, and injecting malicious control prompts into LLM tool outputs, these exercises build critical advanced application security and AI safety skills.

---

## Lab Collection & Index

Below is the complete, searchable index of all web cache desynchronization, HTTP/2 smuggling, parameter ambiguity, and LLM security challenges in this collection:

| # | Lab / Challenge Name | Category | Focus / Key Topics | Lab Link |
|---|----------------------|----------|---------------------|----------|
| 1 | **Web Cache Desynchronization** | Web Cache Poisoning, Deception & Key Manipulation | Front-end/back-end cache key mismatches, unkeyed header injection, persistent cache poisoning, XSS delivery via cache | [Access Lab](https://learn.secbyte.org/ctf/web-cache-desynchronization) |
| 2 | **Web Cache Entanglement** | Web Cache Poisoning, Deception & Key Manipulation | Multiple cache layer interactions, fat GET requests, unkeyed port/host parameters, complex cache poisoning chains | [Access Lab](https://learn.secbyte.org/ctf/web-cache-entanglement) |
| 3 | **Cache Key Confusion** | Web Cache Poisoning, Deception & Key Manipulation | URL path normalization differences, unkeyed query parameters, origin vs. cache key transformation flaws | [Access Lab](https://learn.secbyte.org/ctf/cache-key-confusion) |
| 4 | **HTTP Cache Deception: Learning Room** | Web Cache Poisoning, Deception & Key Manipulation | Static file extension path manipulation (`/profile.php/nonexistent.css`), caching dynamic user data, sensitive account leaks | [Access Lab](https://learn.secbyte.org/ctf/http-cache-deception-learning-room) |
| 5 | **HTTP/2 Request Smuggling** | HTTP/2 Smuggling, Protocol Attacks & DoS | HTTP/2 to HTTP/1.1 downgrade request smuggling, H2.TE / H2.CL desynchronization, request queue poisoning, session hijacking | [Access Lab](https://learn.secbyte.org/ctf/http2-request-smuggling) |
| 6 | **HTTP/2 Rapid Reset: Detection & Defense** | HTTP/2 Smuggling, Protocol Attacks & DoS | CVE-2023-44487 stream cancellation abuse (`RST_STREAM` frame flooding), server resource exhaustion, DoS detection & mitigation | [Access Lab](https://learn.secbyte.org/ctf/http2-rapid-reset-detection-defense) |
| 7 | **HTTP Verb Tampering** | HTTP Parameter & Verb Tampering, Host Headers | Bypassing verb-based access controls (GET vs. POST vs. HEAD/OPTIONS), authentication filter bypass, unauthorized action execution | [Access Lab](https://learn.secbyte.org/ctf/http-verb-tampering) |
| 8 | **HTTP Method Override Abuse: Hidden Verb Escalation** | HTTP Parameter & Verb Tampering, Host Headers | Abusing `X-HTTP-Method-Override`, `X-Method-Override`, and `_method` parameters, REST API permission escalation | [Access Lab](https://learn.secbyte.org/ctf/http-method-override-abuse-hidden-verb-escalation) |
| 9 | **HTTP Parameter Fragmentation: From Confusion to Control** | HTTP Parameter & Verb Tampering, Host Headers | Splitting parameter values across headers/body, WAF bypass, backend parser recombination tricks | [Access Lab](https://learn.secbyte.org/ctf/http-parameter-fragmentation-from-confusion-to-control) |
| 10 | **HTTP Parameter Pollution: Parsing Ambiguity & Access Control Bypass** | HTTP Parameter & Verb Tampering, Host Headers | Multi-parameter precedence flaws (first vs. last value), WAF evasion, business logic manipulation, query string override | [Access Lab](https://learn.secbyte.org/ctf/http-parameter-pollution-parsing-ambiguity-access-control-by) |
| 11 | **Host Header Poisoning** | HTTP Parameter & Verb Tampering, Host Headers | `X-Forwarded-Host` / `Host` header manipulation, password reset link poisoning, web cache poisoning via host headers | [Access Lab](https://learn.secbyte.org/ctf/host-header-poisoning-medium) |
| 12 | **LLM Output Injection: Prompt Abuse & Tool Hijacking** | AI & Large Language Model (LLM) Security | Indirect prompt injection, LLM tool/plugin output manipulation, unauthorized API invocation via autonomous agents, safe prompt defenses | [Access Lab](https://learn.secbyte.org/ctf/llm-output-injection-prompt-abuse-tool-hijacking-safe-defens) |

---

## Categories

### 1. Web Cache Poisoning, Deception & Key Manipulation
Exploit unkeyed request headers, manipulate path normalizations to leak user data via Cache Deception, and cause cache key confusion across reverse proxies and CDNs.
- [Web Cache Desynchronization](https://learn.secbyte.org/ctf/web-cache-desynchronization)
- [Web Cache Entanglement](https://learn.secbyte.org/ctf/web-cache-entanglement)
- [Cache Key Confusion](https://learn.secbyte.org/ctf/cache-key-confusion)
- [HTTP Cache Deception: Learning Room](https://learn.secbyte.org/ctf/http-cache-deception-learning-room)

### 2. HTTP/2 Smuggling, Protocol Attacks & Denial of Service
Dissect HTTP/2 protocol frames, exploit HTTP/2-to-HTTP/1.1 downgrade desynchronizations for request smuggling, and analyze HTTP/2 Rapid Reset stream floods.
- [HTTP/2 Request Smuggling](https://learn.secbyte.org/ctf/http2-request-smuggling)
- [HTTP/2 Rapid Reset: Detection & Defense](https://learn.secbyte.org/ctf/http2-rapid-reset-detection-defense)

### 3. HTTP Parameter & Verb Tampering, Host Header Poisoning
Bypass web application firewalls and authorization filters using verb tampering, method override headers, parameter pollution (HPP), parameter fragmentation, and host header poisoning.
- [HTTP Verb Tampering](https://learn.secbyte.org/ctf/http-verb-tampering)
- [HTTP Method Override Abuse: Hidden Verb Escalation](https://learn.secbyte.org/ctf/http-method-override-abuse-hidden-verb-escalation)
- [HTTP Parameter Fragmentation: From Confusion to Control](https://learn.secbyte.org/ctf/http-parameter-fragmentation-from-confusion-to-control)
- [HTTP Parameter Pollution: Parsing Ambiguity & Access Control Bypass](https://learn.secbyte.org/ctf/http-parameter-pollution-parsing-ambiguity-access-control-by)
- [Host Header Poisoning](https://learn.secbyte.org/ctf/host-header-poisoning-medium)

### 4. AI & Large Language Model (LLM) Security
Study security boundaries in integrated LLM agents, executing indirect prompt injections to hijack tool function calls and manipulate AI system outputs.
- [LLM Output Injection: Prompt Abuse & Tool Hijacking](https://learn.secbyte.org/ctf/llm-output-injection-prompt-abuse-tool-hijacking-safe-defens)

---

## Learning Path

Follow this structured progression path to master HTTP parameter ambiguity, web cache poisoning/deception, HTTP/2 protocol smuggling, and LLM output safety:

1. **Phase 1: HTTP Parameter Ambiguity, Verb Tampering & Host Header Poisoning** — Master HTTP verb overrides, parameter precedence bugs, and host header injection vectors:
   - [HTTP Verb Tampering](https://learn.secbyte.org/ctf/http-verb-tampering)
   - [HTTP Method Override Abuse: Hidden Verb Escalation](https://learn.secbyte.org/ctf/http-method-override-abuse-hidden-verb-escalation)
   - [HTTP Parameter Pollution: Parsing Ambiguity & Access Control Bypass](https://learn.secbyte.org/ctf/http-parameter-pollution-parsing-ambiguity-access-control-by)
   - [HTTP Parameter Fragmentation: From Confusion to Control](https://learn.secbyte.org/ctf/http-parameter-fragmentation-from-confusion-to-control)
   - [Host Header Poisoning](https://learn.secbyte.org/ctf/host-header-poisoning-medium)

2. **Phase 2: Web Cache Poisoning & HTTP Cache Deception** — Exploit unkeyed headers and cache key normalizations to poison web caches and leak sensitive user profiles:
   - [HTTP Cache Deception: Learning Room](https://learn.secbyte.org/ctf/http-cache-deception-learning-room)
   - [Cache Key Confusion](https://learn.secbyte.org/ctf/cache-key-confusion)
   - [Web Cache Desynchronization](https://learn.secbyte.org/ctf/web-cache-desynchronization)
   - [Web Cache Entanglement](https://learn.secbyte.org/ctf/web-cache-entanglement)

3. **Phase 3: HTTP/2 Protocol Smuggling & Stream Resets** — Craft HTTP/2 frame sequences to smuggle requests across front-end reverse proxies and analyze rapid reset DoS:
   - [HTTP/2 Request Smuggling](https://learn.secbyte.org/ctf/http2-request-smuggling)
   - [HTTP/2 Rapid Reset: Detection & Defense](https://learn.secbyte.org/ctf/http2-rapid-reset-detection-defense)

4. **Phase 4: AI & LLM Agent Safety (Indirect Prompt Injection)** — Craft malicious data payloads to hijack autonomous LLM agent tool calling and API executions:
   - [LLM Output Injection: Prompt Abuse & Tool Hijacking](https://learn.secbyte.org/ctf/llm-output-injection-prompt-abuse-tool-hijacking-safe-defens)

---

## How to Use the Labs

1. Select a challenge link from the index or category sections above.
2. Read the scenario directives, protocol specifications, and target parameters on [Learn SecByte](https://learn.secbyte.org/).
3. Deploy analysis toolsets (Burp Suite Pro with HTTP Request Smuggler / Param Miner, Python, Curl, Go H2 framing scripts) inside an isolated workstation.
4. Inject unkeyed headers, send HTTP/2 request smuggling frames, manipulate cache paths, craft indirect LLM prompt injections, and capture target flags.

---

## Disclaimer

This repository and its linked challenge resources are strictly intended for educational, threat research, and authorized technical security training purposes. Never execute web cache poisoning attacks, HTTP/2 request smuggling, stream reset floods, or prompt injections against unauthorized production web applications, live CDNs, or third-party AI integrations.
