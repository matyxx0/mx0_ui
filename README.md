# mx0_ui

UI bridge and shared styling for mx0 scripts.

## Overview

`mx0_ui` is a small bridge resource meant to keep UI styling consistent across mx0 scripts. 

Instead of opening every single script and editing CSS files one by one just to change primary colors or dark mode shades, this script acts as a central place for your UI themes. It basically contains just `fxmanifest.lua` and a global `colors.css`.

When you update `colors.css` here, every mx0 script connected to it automatically adapts to the new palette.

---

## Is this required?

**No, this script is NOT strictly required, but it is strongly recommended** if you are using multiple scripts from the mx0 series—such as:

* Boosting Tablet
* Company Tablet
* Multijob
* Reports System
* ...and other mx0 UI resources.

If you only run one script, you can easily embed the CSS directly into that resource. But if you run a full suite of mx0 scripts, having this installed saves you from repetitive file editing whenever you want to rebrand or adjust your UI colors.

---

## How to use it

1. Drop `mx0_ui` into your server's `resources` folder.
2. Start it in your `server.cfg` before any other mx0 resources:

```cfg
ensure mx0_ui
ensure mx0_boosting
ensure mx0_multijob
# ...other scripts
