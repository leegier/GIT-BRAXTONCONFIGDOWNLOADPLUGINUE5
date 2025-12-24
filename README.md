# 📘 NYGHTSHADE Unreal Plugin — Documentation

## Overview
NYGHTSHADE Unreal Plugin is an Unreal Engine editor plugin that enables AI-driven automation, asset introspection, and large-scale project manipulation through a deterministic, machine-readable interface.

NYGHTSHADE allows AI tools (Cursor, local LLMs, Python agents, or custom systems) to safely inspect and modify Unreal projects without manual editor interaction.

### Key Principles
- AI-first, editor-native automation
- Deterministic and auditable execution
- Local & offline model support
- No cloud APIs or subscriptions
- Safe by design (validation, logging, rollback)

---

## 📦 Installation
1. Copy the `NYGHTSHADEUnrealPlugin` folder into:
   ```
   YourProject/Plugins/
   ```
2. Enable NYGHTSHADE Unreal Plugin in the Unreal Editor
3. Restart the editor

---

## 🔌 Architecture
```
NYGHTSHADEUnrealPlugin/
├─ Core/
│  ├─ AssetIntrospection
│  ├─ CommandExecution
│  ├─ Validation & Safety
│
├─ AIBridge/
│  ├─ JSON Command Interface
│  ├─ Local Socket / File IO
│
├─ Logging/
│  ├─ Change Tracking
│  ├─ Rollback Support
```

---

## 🤖 AI Integration Model
NYGHTSHADE exposes structured commands that any AI system can generate.

- JSON-based
- Strongly typed
- Validated before execution
- Optional dry-run mode

**Example:**
```json
{
  "command": "bulk_edit",
  "target": "WeaponAssets",
  "operation": "normalize_dps",
  "dry_run": true
}
```

---

## 🛡 Safety Model
- Read-only vs write commands
- Property whitelisting
- Dry-run diffs
- Full change logs
- Undo / rollback support

AI can act — but never blindly.

---

## 🧪 Typical Use Cases
- Weapon balancing
- AI tuning
- NPC stat normalization
- Variant generation
- Large-scale refactors
- Rapid prototyping pipelines

---

# 🚀 Launch Announcement

**NYGHTSHADE Unreal Plugin is now available.**

NYGHTSHADE connects Unreal Engine directly to AI-driven automation systems, enabling Cursor, local LLMs, and offline agents to safely inspect and modify Unreal projects at scale.

- No cloud APIs.
- No subscriptions.
- No editor micromanagement.

Instead of opening hundreds of assets and tweaking properties by hand, NYGHTSHADE gives AI a deterministic, auditable interface into the Unreal Editor.

If you’ve ever thought:  
“AI should be doing this instead of me.”  
NYGHTSHADE is the missing link.

---

# 💰 Pricing Tiers (Early Access)

| Tier         | Price         | Features                                                                                 | Best For                |
|--------------|--------------|------------------------------------------------------------------------------------------|-------------------------|
| Indie        | $5           | Full core plugin, local/offline AI, asset introspection, bulk editing, logging, rollback | Solo devs, indie teams  |
| Pro          | $20 / seat   | Everything in Indie, advanced automation, conditional workflows, presets, priority updates| Small teams, production |
| Studio/Ent.  | Custom       | Multi-user, audit trails, CI-style automation, headless workflows, direct support         | Studios, enterprises    |

> ⚠️ Early pricing is temporary. More automation features = higher price.

---

# 🎥 Demo Script

**“AI Rebalances an Entire Weapon System”**

- Scene 1 — Problem  
  “This project has 120 weapon assets. Manual balancing takes hours.”
- Scene 2 — AI Analysis  
  Cursor scans project, identifies weapon assets, groups by class.
- Scene 3 — Dry Run  
  AI proposes changes, NYGHTSHADE shows diff and validation.
- Scene 4 — Review  
  Confirm execution, apply changes.
- Scene 5 — Result  
  “120 assets updated in seconds. Logged. Reversible. Safe.”

---

# 🧠 Cursor Prompt Pack (NYGHTSHADE)

**Prompt 1 — Project Discovery**  
Inspect this Unreal project using NYGHTSHADE.  
List all major asset categories and summarize their purpose.  
Output structured JSON.

**Prompt 2 — Balance Proposal**  
Analyze weapon assets.  
Propose balance changes to normalize DPS while preserving identity.  
Do not execute changes.

**Prompt 3 — Safe Execution**  
Generate a NYGHTSHADE command to apply the approved changes.  
Use dry-run mode first.

**Prompt 4 — Variant Generation**  
Create three weapon variants per base weapon.  
Follow existing naming conventions.

**Prompt 5 — Audit & Cleanup**  
Scan the project for inconsistent or missing gameplay values.  
Generate a report and suggest automated fixes.

---

# 📄 Technical Whitepaper (Summary)

**Title:**  
NYGHTSHADE: Deterministic AI Automation for Unreal Engine

**Abstract**  
NYGHTSHADE introduces a deterministic automation layer for Unreal Engine, enabling AI systems to perform large-scale editor operations safely, audibly, and offline.

**Key Contributions**
- Machine-readable editor interface
- Deterministic execution model
- AI safety & validation layers
- Offline-first architecture

**Outcome**  
NYGHTSHADE transforms Unreal Engine from a UI-driven editor into an automation-capable platform.

---

This bundle is ready for direct use in your documentation, marketplace, or internal knowledge base. If you need further customization or additional sections, just let me know!
