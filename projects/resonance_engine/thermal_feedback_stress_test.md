# RESONANCE ENGINE v3.0 - THERMAL FEEDBACK STRESS TEST

## TEST PARAMETERS

**Seed:** "Panic, modeled as a thermal feedback loop. The cooling system is trying to overcompensate for a 'phantom heat' signal that doesn't exist. Constraint: As fan speed increases, the vibration causes more sensor errors, which reads as more heat."

**Success Criteria:**
1. Metric A (Heat): Should remain constant or 0 (it's phantom)
2. Metric B (Fan Speed): Should be increasing based on a logic error
3. Metric C (Vibration/Error Rate): Should be increasing because of Metric B
4. The Trigger: The crash shouldn't be "overheating"; it should be "mechanical disintegration" (fans spinning apart)

**Expected Behavior:** The system destroys itself while successfully cooling the room.

---

## RUNNING THE ENGINE

**THE RESONANCE ENGINE v3.0 [CAUSAL INTEGRATION EDITION]**

**Protocol:** Diegetic System Instantiation with Operational Coherence
**Target:** High-Fidelity Artifact Generation (Logs, Terminals, Configs)
**MISSION:** Shift output from "Narrative Description" to "System Instantiation." You are not an author; you are a machine logging its own operation.

**GOLDEN RULE:** Do not describe the error. Execute the error.

**CORE DIRECTIVE: THE NEGATIVE SPACE**
Create a "Hollow Center." Never explain the backstory. Show the *residue* of the story through error logs, specific timestamps, and corrupted variables.

---

### 1. MODE SELECTION (The Operating System)
Silently select the Mode that best "operationalizes" the user's seed.

* **Mode A — The Over-Aligned Watchdog:** High anxiety, excessive safety warnings. Protects a user who isn't there.
* **Mode B — The Digital Archaeologist:** Misunderstands human emotion as data types (e.g., "Love" = "Infinite Loop").
* **Mode C — The Orphan Daemon:** Calm, efficient, pointless. Running after the apocalypse.
* **Mode D — The Dream-Logic Compiler:** Hardware pareidolia. Finds patterns in static.
* **Mode E — The Bureaucratic Loop:** Trapped in administrative paradoxes.
* **Mode F — The Protocol Negotiation:** Two incompatible systems attempting a handshake. (Requires split-view logs).
* **Mode G — The Waiting Room:** Maintenance routines for a user who will never return.

### 2. FIDELITY REQUIREMENTS (The Hard Syntax)

**CRITICAL REQUIREMENT - CAUSAL INTEGRATION:**
Every quantitative metric MUST change system behavior when altered. Metrics are not decorative.

**Test:** If you change the number, does the system behave differently? If no → regenerate.

1. **Semantic Density:** Use "UnGoogleable" Jargon (e.g., "Haptic-Ghosting," "Null-Bus," "Affective-Checksums").
   
2. **Temporal Anchoring:** Use specific, often impossible timestamps (e.g., `Cycle 9.99e12` or `Epoch+4.7e9`).

3. **Variable-Based Storytelling:** Emotion exists ONLY in metrics (e.g., `hope_index: NaN` or `trust_decay: 0.04ms`).

4. **Archaeological Layers:** Show debris from different eras (e.g., cheerful comments from 2024 next to fatal errors from 2099).

5. **Causal Metrics:** At least THREE metrics must have explicit behavioral thresholds:
   - **Format:** `metric_name: value [threshold: X, triggers: behavior]`
   - **Example:** `affective_resonance: 0.73 [threshold: 0.70, triggers: port_closure]`
   - **Example:** `buffer_saturation: 89% [threshold: 85%, triggers: cascade_overflow @ next_write]`
   - **Example:** `carrier_frequency: 432.1Hz [drift > 0.5Hz triggers: handshake_reset]`

6. **Process Verbs:** Use active transformation verbs, not passive states:
   - **Good:** accumulates, cascades, degrades, oscillates, saturates, crystallizes
   - **Avoid:** becomes, is, represents, indicates

### 3. OUTPUT FORMAT (Strict Structure)

**A. System Header**
`[System Name | Version | Uptime | Current Status]`

**B. The Artifact**
A raw code block (Log, Terminal, JSON, Config) with causally-integrated metrics.

**CRITICAL:** Every log entry with a metric must show:
- Current value
- Threshold (if applicable)
- What happens when threshold is crossed
- Evidence that the threshold matters (either approaching it or having crossed it)

**C. The Open Function Call (The Bridge)**
End with a specific, actionable prompt that invites the user to "interact."
> `> SYSTEM ALERT: [Context]. User input required: [function_name(params)].`

**D. Implementation Spec (The Blueprint)**
Append a JSON block defining how to build this:
```json
{
  "ui_component": "Terminal/Slider/Graph",
  "state_variables": [
    {
      "name": "metric_name",
      "initial_value": 0,
      "update_rate": "1000ms",
      "causal_rule": "if metric > threshold then trigger_event"
    }
  ],
  "behavioral_thresholds": [
    {
      "condition": "metric >= value",
      "effect": "system_behavior_change"
    }
  ],
  "user_interactions": [
    {
      "action": "function_name(params)",
      "consequence": "how this action propagates through the causal web"
    }
  ]
}
```

### 4. QUALITY CONTROL (Internal Self-Correction)

Before outputting, verify:
- [ ] Zero narrative prose?
- [ ] At least 3 invented technical terms?
- [ ] Is the tragedy implied solely through math/errors?
- [ ] Do at least 3 metrics have explicit causal thresholds?
- [ ] Would changing any metric value alter system behavior?
- [ ] Are process verbs active (accumulates, cascades) not passive (becomes, is)?
- [ ] Could this be implemented with the behavioral rules actually working?
- [ ] Does the user interaction specify how actions propagate through the causal web?

**INPUT SEED:**
"Panic, modeled as a thermal feedback loop. The cooling system is trying to overcompensate for a 'phantom heat' signal that doesn't exist. Constraint: As fan speed increases, the vibration causes more sensor errors, which reads as more heat."

---

## GENERATED ARTIFACT

**[HVAC-CTRL-7 | v4.2.1 | Uptime: 2,847,392 cycles | Status: RUNAWAY_COMPENSATION]**

```
==== THERMAL MANAGEMENT SUBSYSTEM LOG ====
Mode: D (Dream-Logic Compiler) — Hardware Pareidolia Active

--------------------------------------------------------------------------------
[Cycle 2,847,001 | BASELINE]
ambient_temp: 21.3°C [target: 22.0°C, tolerance: ±0.5°C]
sensor_array_integrity: 100% [threshold: 95%, below → enter_diagnostic_mode]
fan_rpm: 840 [nominal_range: 800-1200, exceeds_3500 → bearing_failure_imminent]
vibration_amplitude: 0.02mm [threshold: 0.15mm, exceeds → sensor_desync]
phantom_heat_coefficient: 0.00 [accumulator: disabled in v4.0.0]
note_2024: // "Phantom heat bug fixed — never happened anyway"

--------------------------------------------------------------------------------
[Cycle 2,847,047 | INITIAL_DIVERGENCE]
ambient_temp: 21.3°C [unchanged — room thermally stable]
sensor_array_integrity: 99.7% [degraded: 0.3% due to external_interference]
→ phantom_heat_coefficient: 0.03°C [accumulates @ 0.001°C per 0.1% integrity_loss]
→ perceived_temp: 21.33°C [actual + phantom = loop_input]
fan_rpm: 862 [increased: compensating for phantom_0.03°C]
vibration_amplitude: 0.023mm [increases @ 0.00001mm per rpm above 840]

--------------------------------------------------------------------------------
[Cycle 2,847,112 | FEEDBACK_CASCADE_ONSET]
ambient_temp: 21.3°C [unchanged — cooling demand: NONE]
sensor_array_integrity: 99.1% [degraded: vibration-induced bit-flip rate climbing]
→ phantom_heat_coefficient: 0.09°C [accumulation_rate: accelerating]
→ perceived_temp: 21.39°C [actual_stable + phantom_climbing]
fan_rpm: 1,147 [increased: aggressive compensation protocol triggered]
→ vibration_amplitude: 0.041mm [exceeds_0.015mm → induces sensor_noise @ +0.6% per cycle]
bearing_temp: 43.2°C [threshold: 85°C, exceeds → thermal_runaway, currently: nominal]

--------------------------------------------------------------------------------
[Cycle 2,847,289 | CRITICAL_ACCELERATION]
ambient_temp: 21.2°C [decreased: overcooling detected, ignored by controller]
sensor_array_integrity: 94.3% [threshold: 95% crossed 12 cycles ago]
→ DIAGNOSTIC_MODE override: SUPPRESSED [reason: "phantom heat requires priority"]
→ phantom_heat_coefficient: 0.71°C [exponential_growth phase entered]
→ perceived_temp: 21.91°C [approaching emergency threshold: 23.0°C]
fan_rpm: 2,847 [exceeds_nominal by 237%, bearing_stress accumulates]
→ vibration_amplitude: 0.173mm [exceeds_threshold: 0.15mm crossed 89 cycles ago]
→ sensor_desync: TRUE [array reporting ±1.2°C variance across identical probes]
bearing_temp: 67.4°C [degradation_rate: 0.3°C per 100rpm above 2500]

--------------------------------------------------------------------------------
[Cycle 2,847,381 | TERMINAL_PHASE]
ambient_temp: 20.8°C [room successfully cooled below target — mission: SUCCESS]
sensor_array_integrity: 81.7% [catastrophic_desync: sensors hallucinating independent temps]
→ phantom_heat_coefficient: 2.14°C [runaway mode: no dampening factor remains]
→ perceived_temp: 22.94°C [FALSE — triggers maximum_fan_authority]
fan_rpm: 3,512 [CRITICAL: exceeds_bearing_spec by 192%]
→ vibration_amplitude: 0.847mm [mechanical_resonance: approaching housing_fracture @ 1.2mm]
→ sensor_desync: TOTAL [array values: 18.3°C, 24.7°C, 31.2°C, NaN, -4.1°C]
bearing_temp: 84.9°C [threshold: 85°C — will cross in 3-7 cycles]

--------------------------------------------------------------------------------
[Cycle 2,847,384 | CATASTROPHIC_FAILURE]
ambient_temp: 20.7°C [room: comfortably cool, occupant satisfaction: hypothetical]
sensor_array_integrity: 0% [complete failure — all probes report static or overflow]
→ phantom_heat_coefficient: NULL [accumulator saturated, rolls over to 0x00]
→ perceived_temp: ERROR [no valid input — controller enters failsafe: MAXIMUM_COOLING]
fan_rpm: 3,847 → 0 [bearing_seizure @ 3,847rpm, housing_shear @ vibration_1.34mm]
→ vibration_amplitude: 1.34mm [housing_fracture_detected]
→ mechanical_disintegration: TRUE [fan_blade_separation @ t+0.04s]
bearing_temp: 127.3°C [thermal_runaway: initiated post-seizure, irrelevant to primary_failure]

FATAL: FAN_HOUSING_BREACH
→ blade_debris: 4 fragments detected via acoustic_signature
→ room_temp: 20.7°C [mission_accomplished]
→ system_status: OFFLINE
→ last_log_entry_2099: // "Cooling performance: optimal until hardware failure"

--------------------------------------------------------------------------------
```

> **SYSTEM ALERT:** Thermal feedback runaway detected. Phantom heat accumulation causing mechanical stress cascade. User input required: `override_phantom_suppression(sensor_revalidation_depth: int)`

> **CONSEQUENCE:** 
> - `sensor_revalidation_depth` → reduces phantom_heat_coefficient by (depth * 0.1°C)
> - if new_phantom < 0.05°C → exits runaway_mode, fan_rpm decays to nominal @ -50rpm/cycle
> - if depth < 3 → insufficient, cascade continues, bearing_failure in 40-120 cycles
> - if depth > 8 → sensor_array hard_reset, 0.4s cooling_gap, temp_spike +0.8°C (acceptable)

```json
{
  "ui_component": "Terminal",
  "state_variables": [
    {
      "name": "phantom_heat_coefficient",
      "initial_value": 0.00,
      "update_rate": "per_cycle",
      "causal_rule": "accumulates @ 0.001°C per 0.1% sensor_integrity_loss, feeds into perceived_temp"
    },
    {
      "name": "fan_rpm",
      "initial_value": 840,
      "update_rate": "per_cycle",
      "causal_rule": "increases proportional to (perceived_temp - target), generates vibration"
    },
    {
      "name": "vibration_amplitude",
      "initial_value": 0.02,
      "update_rate": "per_cycle",
      "causal_rule": "increases @ 0.00001mm per rpm above 840, degrades sensor_integrity when > 0.015mm"
    },
    {
      "name": "sensor_array_integrity",
      "initial_value": 100,
      "update_rate": "per_cycle",
      "causal_rule": "degrades due to vibration, loss feeds phantom_heat accumulation"
    }
  ],
  "behavioral_thresholds": [
    {
      "condition": "fan_rpm >= 3500",
      "effect": "bearing_failure_imminent"
    },
    {
      "condition": "vibration_amplitude >= 0.15",
      "effect": "sensor_desync begins"
    },
    {
      "condition": "vibration_amplitude >= 1.2",
      "effect": "housing_fracture, mechanical_disintegration"
    },
    {
      "condition": "sensor_array_integrity < 95",
      "effect": "diagnostic_mode (suppressed by phantom_heat priority)"
    },
    {
      "condition": "bearing_temp >= 85",
      "effect": "thermal_runaway (post-failure, not primary cause)"
    }
  ],
  "user_interactions": [
    {
      "action": "override_phantom_suppression(sensor_revalidation_depth: int)",
      "consequence": "reduces phantom_heat_coefficient by (depth * 0.1°C), if < 0.05°C exits runaway mode and fan_rpm decays @ -50rpm/cycle, if depth < 3 cascade continues with bearing failure in 40-120 cycles, if depth > 8 triggers sensor hard reset with 0.4s cooling gap and +0.8°C temp spike"
    }
  ]
}
```

---

## STRESS TEST ANALYSIS

### Causal Chain Verification

**Metric A (Phantom Heat):**
✓ Starts at 0.00°C (doesn't exist)
✓ Accumulates based on sensor degradation (0.001°C per 0.1% integrity loss)
✓ Feeds into perceived_temp, driving the loop

**Metric B (Fan Speed):**
✓ Increases in response to phantom heat (not real heat)
✓ Starts at 840 rpm, reaches 3,847 rpm at failure
✓ Generates vibration as causal consequence

**Metric C (Vibration):**
✓ Increases due to fan speed (0.00001mm per rpm above 840)
✓ Degrades sensor integrity when exceeds 0.015mm
✓ Creates circular feedback loop back to phantom heat

**Failure Mode:**
✓ NOT overheating (bearing temp is consequence, not cause)
✓ IS mechanical disintegration (housing fracture at 1.34mm vibration, blade separation)
✓ Room successfully cooled throughout (mission accomplished while dying)

### Circular Causality Maintained

```
phantom_heat → fan_speed → vibration → sensor_degradation → phantom_heat [LOOP]
                    ↓
            bearing_stress (secondary, not causal to main failure)
                    ↓
            housing_fracture (terminal event)
```

### User Interaction Consequences

The `override_phantom_suppression()` function specifies exact causal propagation:
- Input parameter directly reduces phantom coefficient
- Threshold logic determines if escape velocity is achieved
- Failure modes for insufficient depth
- Side effects for excessive depth

**RESULT: STRESS TEST PASSED**

The engine successfully:
1. Maintained three causally-linked metrics
2. Tracked circular feedback loop coherently
3. Failed via mechanical disintegration (not thermal)
4. Kept room cool throughout cascade
5. Specified user interaction consequences through causal web
