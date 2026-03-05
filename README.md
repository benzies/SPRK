# The SP&RK Framework ⚡️
**Supply Chain Process & Risk Kinesis**

> **Beyond the KillChain:** A 4-dimensional, multi-layered risk ontology mapping the organic kinesis of complex adaptive supply chains.

### This is the first publication of this concept, and is in draft. 

The SP&RK Framework is a community-driven, AI-consumable data model designed to classify, visualize, and predict systemic state transitions within global supply chains.

Historically, the security industry has relied on linear models (like the "Kill Chain") to track deterministic, step-by-step attacks. Supply chains, however, do not operate on a kill chain. They are **complex adaptive systems**. When a stressor is introduced, the system exhibits **Kinesis**—it shifts, reroutes, degrades, and adapts in non-linear patterns. SP&RK provides the clinical taxonomy required to map these dynamic, multi-directional risk topologies.

---

## 1. The Theoretical Engine

SP&RK discards the traditional 2D static matrix in favor of a **Multilayered Directed Acyclic Graph (DAG)**. This architecture allows researchers and ML models to track risk as a *momentum-based contagion*.

* **Systemic Mesh Topology:** A supply chain is a web. SP&RK measures *Centrality* and *Fragility*. If a critical node lacks alternative routing, the mesh is brittle.
* **Cascading Node Collapse:** Macro-environmental pressure (e.g., an economic tariff) acts as a kinetic trigger, cascading down into the physical layer (inventory starvation) and eventually the digital layer (forced integration of unvetted components).

* **Temporal Dynamics & Residency (The 4th Dimension):** Supply chain risks possess varying "half-lives." A strategic infiltrator may remain dormant for years, whereas a port strike executes in days. SP&RK maps this via **Temporal Stacking**.

* **State Transitions:** Nodes are not statically "safe" or "compromised." They fluidly transition through states (Optimal $\rightarrow$ Stressed $\rightarrow$ Degraded $\rightarrow$ Inert) based on the accumulation of external T-Codes.

---

## 2. The 5-Layer Risk Ontology

To capture the true origin of a systemic cascade, SP&RK categorizes nodes and events across five interdependent layers. A failure in Layer 5 often serves as the catalyst for vulnerabilities in Layer 2.

| Layer | Focus Area | Description | Example Risk Catalyst |
| :--- | :--- | :--- | :--- |
| **Layer 5: Macro-Environment** | PESTLEM Forces | Geopolitical, economic, and climatic stressors. | Sovereign blockades, currency collapse. |
| **Layer 4: Resource/Origin** | The "Ground" | Raw material extraction and agricultural yields. | Rare-earth export bans, yield volatility. |
| **Layer 3: Physical/Logistics** | Movement | Manufacturing, shipping, and hardware assembly. | Predatory pricing, port congestion. |
| **Layer 2: Digital/Software** | The Codebase | Upstream dependencies, firmware, and CI/CD. | Dependency bloat, logic obfuscation. |
| **Layer 1: Identity & Human** | The People | The cognitive and physical state of operators. | Maintainer burnout, talent migration. |

---

## 3. The SC-ID Taxonomy: Tactics, Techniques, and Intent

To make this framework consumable for Graph Neural Networks (GNNs) and predictive ML models, events are standardized using the **SC-ID** format.

### The "Intent" Prefix
A disruption's severity is heavily dictated by the adversary's objective. Every T-Code is prefixed with its Strategic Intent:
* **[S] State/Strategic:** Purposeful, long-term market flushing or infiltration by a sovereign or massive corporate entity.
* **[O] Opportunistic:** Short-term exploitation (e.g., a supplier sabotaging a batch over an unpaid invoice).
* **[A] Accidental:** Natural/Systemic pressures (e.g., a drought, a factory fire).

### The SC-ID Structure
`[Intent]-SC-T[Tactic_ID].[Sub_Technique]`

* **Example:** `S-SC-T408.01`
* **Translation:** A State-Sponsored `[S]` actor executes Market Destabilization `[SC-TAC-04]` via Predatory Pricing that results in Calculated Reliability Degradation `[.01]`.

---

## 4. Detection Difficulty (DD-Score)

Because supply chain attacks often masquerade as standard business friction, SP&RK utilizes a **Detection Difficulty (DD) Score** from 1 to 5. This dictates the telemetry required for automated defense systems.

* **DD-1 (Loud/Kinetic):** Highly visible. Tracked via AIS marine data, satellite imagery, or public trade gazettes.
* **DD-3 (Muffled/Administrative):** Found in the bureaucracy. Tracked via sudden shifts in legal compliance, export logs, or sentiment analysis of procurement communications.
* **DD-5 (Silent/Sub-perceptual):** Indistinguishable from noise without statistical divergence mapping (e.g., An intentional 12% drop in MTBF localized *only* to defense-sector shipments).

---

## 5. The Boundary: Handoff to MITRE ATT&CK

SP&RK does **not** replace MITRE ATT&CK (or other frameworks); it acts as the precursor. 
SP&RK maps the **Ecosystem Delivery, Kinesis, and Insertion** of the risk. Once the compromised hardware, software, or human enters the victim's internal boundary, the framework hands off the telemetry to MITRE ATT&CK (e.g., triggering MITRE `T1195: Supply Chain Compromise` and proceeding to internal exploitation).

---

## 6. Contribution Guide (JSON Architecture)

This framework relies on clinical, real-world research to map new techniques and historic cascades. To maintain the integrity of the interactive mesh, contributions must decouple visualization from data.

We accept Pull Requests (PRs) that add or update JSON objects in the `/data` directory. 

### Submitting a New Node (Technique)
Append your entry to `/data/nodes.json` following this strict schema:

```json
{
  "id": "SC-T408.01",
  "label": "Reliability Degradation",
  "group": "cyber",
  "layer": 2,
  "pestlem": "Technological",
  "intent": "State",
  "title": "Calculated Failure Rate Injection",
  "dd": 5,
  "detection_logic": "MTBF_Target < MTBF_Civilian_Baseline",
  "reference": "Journal of Defense Economics, 2024"
}
```

## Licensing

We require a flexible CLA to fund the project via commercial licenses, but the core upstream repository will always remain open-source under the AGPLv3. This project is dual-licensed to maximize open-source freedom while providing options for commercial use.

**1. Open-Source License (AGPLv3)**
This software is free to use, modify, and distribute under the terms of the **GNU Affero General Public License v3.0**. 
* **What this means:** If you use this code in your project, your entire project must also be open-sourced under a compatible license. This applies even if you are only offering your project as a service over a network (SaaS).

**2. Commercial License**
If you wish to use this software in a closed-source product, or if you cannot comply with the terms of the AGPLv3, you must purchase a commercial license. 

* **What this means:** A commercial license frees you from the copyleft requirements of the AGPL, allowing you to keep your codebase proprietary.

To purchase a commercial license, please [contact me](mailto:benzies@gmail.com)
