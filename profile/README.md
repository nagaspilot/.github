<div align="center" style="text-align: center;">

<h1>NagasPilot</h1>

<p>
  <b>NagasPilot is a fork of openpilot focusing on Chinese car brands.</b>
  <br>
  Based in Thailand, we port openpilot to Chinese vehicles lacking support in the US market.
</p>

</div>

Hardware Architecture
------

### Universal Protocol Standard

For maximum hardware compatibility, NagasPilot implements a common control protocol based on **Tesla Model 3 standard CAN bus** (500 kbps, non-CAN-FD). This design choice ensures compatibility with Comma 3 classic and newer devices while maintaining broad vehicle support.

### Gateway Technology (brownpanda)

NagasPilot utilizes a specialized **automotive gateway hardware (brownpanda)** that translates between vehicle-specific protocols and our universal Tesla-based protocol. This approach enables:

- **Hardware Safety**: AEC-Q100 grade automotive microcontrollers with fail-safe fallback mechanisms
- **Universal Compatibility**: Support for any vehicle brand while maintaining openpilot source compatibility
- **User Safety**: Integrated physical switch allowing instant system deactivation—factory OEM ADAS remains functional when switch is not engaged
- **Enhanced Safety Architecture**: In the enhancedpilot project, ADAS safety logic has been migrated to the gateway hardware (brownpanda), enabling seamless integration and switching between OEM ADAS mode and enhanced/openpilot mode

This architecture provides non-technical users with a simple hardware override mechanism for peace of mind.

---

Our Projects
------

We believe AI cannot solve all driving scenarios. NagasPilot branches into two projects:

- **openpilot**: Fork of DragonPilot Brother for Chinese car compatibility
- **enhancedpilot**: Hybrid rewrite combining rule-based stereo vision with AI-assisted decision making

---

**Requirements:**
- Comma 3 classic or newer hardware
- Chinese EV brands with brownpanda tuning
- Car harness from exo-electronics
- brownpanda automotive gateway with safety switch

**THIS IS ALPHA QUALITY SOFTWARE FOR RESEARCH PURPOSES ONLY. THIS IS NOT A PRODUCT.
YOU ARE RESPONSIBLE FOR COMPLYING WITH LOCAL LAWS AND REGULATIONS.
NO WARRANTY EXPRESSED OR IMPLIED.**
