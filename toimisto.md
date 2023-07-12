---
description: Koodiklinikkalaisten hyväksi havaitsemia toimistotarvikkeita.
---

# Toimistotarvikkeita

## LG C2 42" näyttönä

### Service menu

Service menuun pääsee käsiksi [tällä työkalulla](https://github.com/chros73/bscpylgtv). Vaihda tilalle telkkarin IP (löytyy telkkarin verkkoasetuksista).

Helpottaa HDMI-inputin asettamista PC-tilaan, kun telkkari sen usein unohtaa.

```
# avaa service menun (password 0413)
bscpylgtvcommand 192.168.1.18 launch_app_with_params com.webos.app.factorywin '{"id":"executeFactory", "irKey":"inStart"}'

# sulkee service menun
bscpylgtvcommand 192.168.1.18 button EXIT

# asettaa hdmi2:n pc-moodiin
bscpylgtvcommand 192.168.1.18 set_device_info HDMI_2 pc PC
```

### 4K@120Hz macOS:lla

Linkin takaa ohjeistus, todettu toimivaksi M1-koneilla niin Cable Mattersin kuin Ankerin 7100-chipin sisältävillä adaptereilla

Ref: https://forums.macrumors.com/threads/dp-usb-c-thunderbolt-3-4-to-hdmi-2-1-4k-120hz-rgb4-4-4-10b-hdr-with-apple-silicon-m1-m2-now-possible.2381664/

### HDR

Dynamic Tone Mapping ilmestyy telkkarin kuva-asetuksiin kun HDR-tilan kytkee päälle. Sen päälläolo aiheuttaa kuvan välkkymistä kuvan kirkkauden vaihtelun takia. Kannattaa kytkeä työpöytäkäytössä pois.
