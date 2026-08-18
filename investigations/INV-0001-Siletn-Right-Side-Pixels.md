# INV-0001 — Silent Right-Side Pixels

**Status:** Active  
**Version:** 0.1.0

---

# Purpose

This investigation determines why portions of the Christmas-light display
receive power or data incorrectly after deployment.

The complete display contains more than 7,000 individually addressable pixels
and LEDs. The subsystem presently under investigation includes the arches,
mini trees, stars, extension wiring, xLights output configuration, Raspberry
Pi show player, and mega-tree controller associated with the left-side and
right-side props.

---

# Investigation Timeline

## INV-0001-E001 — Raspberry Pi Access Restored

**Type:** Access Restoration  
**Date:** 2026-08-15

The Raspberry Pi could no longer connect through Wi-Fi because the network
password had changed.

The Raspberry Pi was connected through Ethernet, which is its normal deployed
network connection. Access to the Raspberry Pi was successfully restored.

No conclusion concerning the pixel failures was produced by this event.

## INV-0001-E002 — xLights Output Assignment Discovered

**Type:** Configuration Observation  
**Date:** 2026-08-15

Inspection of the xLights configuration revealed that an earlier
troubleshooting change had divided the left and right display halves across
two controller outputs.

Both halves are controlled by the same deployed controller. Use of the same
controller does not establish that both halves use the same physical output
port.

The logical xLights output assignments have not yet been completely reconciled
with the deployed physical wiring.

This observation invalidated the earlier assumption that the complete failure
could be investigated solely as one continuous signal path through the
12-foot extension.

## INV-0001-E003 — Detailed Prop Behavior Observed

**Type:** Observation  
**Date:** 2026-08-15

The following behavior was observed:

| Display location | Power observation | Response observation |
|---|---|---|
| Left arch of the left-side pair | Power present | Working |
| Right arch of the left-side pair | Power present | Not responding |
| Left arch of the right-side pair | Power present | Working except for its star |
| Right arch of the right-side pair | No power observed | Data response cannot yet be evaluated |

The statement that signal is not passing through the right arch of the
left-side pair remains an interpretation. The directly preserved observation
is that the arch has power but does not respond as intended.

Because the right arch of the right-side pair has no power, no conclusion
about its data signal can presently be justified.

## INV-0001-E004 — Mega-Tree Controller Access Constraint

**Type:** Investigation Constraint  
**Date:** 2026-08-15

The mega-tree controller and related equipment had been taken down because the
garage floor must be prepared for concrete.

Restoring the mega-tree controller to the network may require temporary
physical access around the stored equipment.

No controller configuration was downloaded during this event.

## INV-0001-E005 — Configuration Restoration Planned

**Type:** Test Plan  
**Date:** 2026-08-15

The engineer plans to:

1. restore the mega-tree controller to the network;
2. preserve its present configuration when possible;
3. download the intended xLights output configuration;
4. restart or reboot the applicable controller services;
5. run a known test pattern; and
6. compare prop power and response before and after the configuration download.

The test has not yet been performed.

## INV-0001-E006 — Controller Configuration Restored

**Type:** Investigation  
**Date:** 2026-08-15

The Ethernet hub was located, and the mega-tree controller was connected to
the network.

The engineer successfully accessed the controller and carefully inspected its
input and output configuration. After that inspection, the intended input and
output configuration was downloaded to the controller.

The affected display props were tested after the download. The previously
observed failures remained present.

This result reduces confidence that a missing or stale controller
configuration is the sole cause of the failures. It does not establish that
the logical xLights output assignments correspond to the deployed physical
ports and wiring, nor does it establish that every controller output is
delivering valid power and data.
---

# Current Engineering State

The mega-tree controller is now accessible through Ethernet. Its input and
output configuration was inspected, and the intended configuration was
downloaded successfully.

The download did not change the observed failures:

- one powered arch on the left-side pair does not respond;
- one powered arch on the right-side pair responds except for its star; and
- the remaining right-side arch has no observed power.

A missing or stale controller configuration is therefore less likely to be
the sole explanation.

The remaining uncertainty is divided between:

- the physical correspondence between controller outputs and deployed wiring;
- power delivery to the unpowered arch;
- data delivery to powered but nonresponsive props; and
- damage or changed connections within the affected display sections.

---

# Current Selected Question

> When each affected display section is disconnected from the deployed
> controller and independently supplied with 5 V, ground, and data by the test
> controller, which props respond correctly?

---

# Pending Tests

- Isolate each affected display section from the deployed controller.
- Connect the independently powered test controller directly to the input of
  each affected section.
- Record which pixels and props respond, including the nonresponsive arch,
  the star, and the currently unpowered arch.
- Measure accessible voltage boundaries if a power failure remains.

---

# Completed Tests

- Indoor test-controller operation of the four arches and four mini trees:
  passed before deployment.
- Continuity test of the deployed wiring: passed.
- Mega-tree controller network restoration: completed.
- Controller input and output configuration inspection: completed.
- Download of the intended controller configuration: completed.
- Post-download display test: completed; the previously observed failures
  remained.

---

# Evidentiary Limits

- The current controller configuration has not yet been redownloaded.
- Logical output assignments have not been fully mapped to physical ports.
- The independent test controller has not yet been used in the yard.
- Accessible-boundary voltage measurements have not yet been performed.
- No individual pixel has been demonstrated to be defective.

---

# History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Active | Initial independent investigation record. |
