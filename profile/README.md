<div align="center" style="text-align: center;">

<h1>NagasPilot</h1>

<p>
  <b>NagasPilot is a fork of openpilot focusing on Chinese car brands.</b>
  <br>
  Based in Thailand, we port openpilot to Chinese vehicles lacking support in the US market.
</p>

Quick start: See below video for installation guideline
</div>

<table>
  <tr>
    <td><a href="https://youtu.be/NmBfgOanCyk" title="Video By Greer Viau"><img src="https://github.com/commaai/openpilot/assets/8762862/2f7112ae-f748-4f39-b617-fabd689c3772"></a></td>
    <td><a href="https://youtu.be/VHKyqZ7t8Gw" title="Video By Logan LeGrand"><img src="https://github.com/commaai/openpilot/assets/8762862/92351544-2833-40d7-9e0b-7ef7ae37ec4c"></a></td>
    <td><a href="https://youtu.be/SUIZYzxtMQs" title="A drive to Taco Bell"><img src="https://github.com/commaai/openpilot/assets/8762862/05ceefc5-2628-439c-a9b2-89ce77dc6f63"></a></td>
  </tr>
</table>


Hardware Architecture
------

### Universal Protocol Standard

For maximum hardware compatibility, NagasPilot implements a common control protocol based on **Tesla Model 3 standard CAN bus** (500 kbps, non-CAN-FD). This design choice ensures compatibility with Comma 3 classic and newer devices while maintaining broad vehicle support.

### PandaGateway Technology

NagasPilot utilizes a specialized **automotive gateway hardware** that translates between vehicle-specific protocols and our universal Tesla-based protocol. This approach enables:

- **Hardware Safety**: AEC-Q100 grade automotive microcontrollers with fail-safe fallback mechanisms
- **Universal Compatibility**: Support for any vehicle brand while maintaining openpilot source compatibility
- **User Safety**: Integrated physical switch allowing instant system deactivation—factory OEM ADAS remains functional when switch is not engaged

This architecture provides non-technical users with a simple hardware override mechanism for peace of mind.

---

Our Projects
------

We believe AI cannot solve all driving scenarios. NagasPilot branches into two projects:

### 1. openpilot (Fork of DragonPilot Brother)
Traditional openpilot fork focused on Chinese car compatibility.

| branch           | URL                                    | description                                                                         |
|------------------|----------------------------------------|-------------------------------------------------------------------------------------|
| `jsa`         | https://smiskol.com/fork/nagaspilot/jsa                     | For JiaShi.Ai Hardware                                                 |
| `c3l` | https://smiskol.com/fork/nagaspilot/c3l               | For MrOne.C3L Hardware |

### 2. enhancedpilot (Hybrid Rewrite)
Rewritten openpilot with hybrid stack combining:
- Rule-based stereo camera system
- AI-assisted decision making
- Enhanced perception for complex scenarios

---

**What you need:**
1. **Supported Device:** Comma 3 classic or newer compatible hardware
2. **Supported Car:** Chinese EV brands with PandaGateway tuning
3. **Car Harness:** Purchase from exo-electronics
4. **PandaGateway:** Automotive-grade protocol converter with safety switch

**THIS IS ALPHA QUALITY SOFTWARE FOR RESEARCH PURPOSES ONLY. THIS IS NOT A PRODUCT.
YOU ARE RESPONSIBLE FOR COMPLYING WITH LOCAL LAWS AND REGULATIONS.
NO WARRANTY EXPRESSED OR IMPLIED.**
