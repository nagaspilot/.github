<div align="center" style="text-align: center;">

<h1>DragonPilot</h1>

<p>
  <b>DragonPilot is a community fork of openpilot.</b>
  <br>
  We are focusing on Toyota and Lexus vehicles with enhanced customization options.
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


Using DragonPilot in a car
------

To use DragonPilot in a car, you need four things:
1. **Supported Device:** Comma 3/3X or Comma 2 compatible hardware
2. **Software:** Choose compatible branch below to install during custom software setup
3. **Supported Car:** Primarily Toyota/Lexus, with support for Honda and Hyundai
4. **Car Harness:** a comma car harness to connect to your car

### Branches
| branch           | URL                                    | description                                                                         |
|------------------|----------------------------------------|-------------------------------------------------------------------------------------|
| `release3`         | https://smiskol.com/fork/dp                     | Main C3 branch, updated weekly with stability focus.                                                 |
| `release2` | https://smiskol.com/fork/dp/release2               | C2 optimized version with hardware-specific adjustments. |
| `beta3` | https://smiskol.com/fork/dp/beta3               | Bleeding edge C3 development branch (unstable). |
| `beta2` | https://smiskol.com/fork/dp/beta2               | Bleeding edge C2 development branch (unstable). |
| `release2_e2e` | https://smiskol.com/fork/dp/release2_e2e               | C2 with advanced end-to-end features. |

Further Information
------

DragonPilot is a community project designed for experienced openpilot users seeking advanced customization.
It is a fork of openpilot with many experimental features and tweaks that modify heavily from stock openpilot.
While it maintains focus on Toyota and Lexus vehicles, it also supports Honda and Hyundai with enhanced tuning options.

**Key Features:**
- Always-on lateral control for all supported makes
- Dashcam recording functionality
- Multiple tuning types (PID, INDI, LQR, TORQUE) available for all vehicles
- MapD support for offline navigation assistance
- Dynamic end-to-end longitudinal switching
- Customizable acceleration profiles and following distance modes

Development happens in the official DragonPilot development repository.
There is no dedicated Discord or Slack channel.


Safety and Testing
----

* openpilot observes [ISO26262](https://en.wikipedia.org/wiki/ISO_26262) guidelines, see [SAFETY.md](https://github.com/commaai/openpilot/blob/master/docs/SAFETY.md) for more details.
* openpilot has software-in-the-loop [tests](https://github.com/commaai/openpilot/blob/master/.github/workflows/selfdrive_tests.yaml) that run on every commit.
* The code enforcing the safety model lives in panda and is written in C, see [code rigor](https://github.com/commaai/panda#code-rigor) for more details.
* panda has software-in-the-loop [safety tests](https://github.com/commaai/panda/tree/master/tests/safety).
* Internally, we have a hardware-in-the-loop Jenkins test suite that builds and unit tests the various processes.
* panda has additional hardware-in-the-loop [tests](https://github.com/commaai/panda/blob/master/Jenkinsfile).
* We run the latest openpilot in a testing closet containing 10 comma devices continuously replaying routes.

<details>
<summary>MIT Licensed</summary>

openpilot is released under the MIT license. Some parts of the software are released under other licenses as specified.

Any user of this software shall indemnify and hold harmless Comma.ai, Inc. and its directors, officers, employees, agents, stockholders, affiliates, subcontractors and customers from and against all allegations, claims, actions, suits, demands, damages, liabilities, obligations, losses, settlements, judgments, costs and expenses (including without limitation attorneys' fees and costs) which arise out of, relate to or result from any use of this software by user.

**THIS IS ALPHA QUALITY SOFTWARE FOR RESEARCH PURPOSES ONLY. THIS IS NOT A PRODUCT.
YOU ARE RESPONSIBLE FOR COMPLYING WITH LOCAL LAWS AND REGULATIONS.
NO WARRANTY EXPRESSED OR IMPLIED.**
</details>

<details>
<summary>User Data and comma Account</summary>

By default, openpilot uploads the driving data to our servers. You can also access your data through [comma connect](https://connect.comma.ai/). We use your data to train better models and improve openpilot for everyone.

openpilot is open source software: the user is free to disable data collection if they wish to do so.

openpilot logs the road-facing cameras, CAN, GPS, IMU, magnetometer, thermal sensors, crashes, and operating system logs.
The driver-facing camera and microphone are only logged if you explicitly opt-in in settings.

By using openpilot, you agree to [our Privacy Policy](https://comma.ai/privacy). You understand that use of this software or its related services will generate certain types of user data, which may be logged and stored at the sole discretion of comma. By accepting this agreement, you grant an irrevocable, perpetual, worldwide right to comma for the use of this data.
</details>
