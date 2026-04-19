# Home Assistant

This repository conatins files relating to homassistant. This is currently just blueprints, but could be more in future.

## Current Blueprints

### IKEA Bilresa Scrollwheel - Light Control

Light controller for the IKEA Bilresa Smart Scroll Wheel via Matter.

Cannot be used with the 2-Button Remote!

VARIABLES:
- 3 Scroll Zones: Choose the function (Brightness, Kelvin, RGB, Presets).
- 3 Buttons x 2 Gestures: Choose a specific action for EACH gesture (double click / hold).

Note: single click will always turn the light on or off (toggle).

REQUIREMENTS:

For optimal behavior, the following settings must be applied:
- ENABLE Events: 3,6,9 (in section "Events")
- ENABLE Sensors: 1,2,4,5,7,8 (in section "Diagnostic")
- DISABLE Events: 1,2,4,5,7,8 (in section "Events")
- DISABLE Sensors: 3,6,9 (in section "Diagnostic")

HELPER GROUP:

If controlling multiple lights, please always use a HELPER GROUP!
Directly controlling multiple entities can cause sync issues.

### How to add the blueprint to home assistant

Add the blueprint to home assistant by going to settings -> Automations & Scenes -> Blueprints -> Import Blueprint

or click on the button below to add the blueprint to home assistant (This will take you to the import blueprint page in home assistant)

[![Install Blueprint](https://community-assets.home-assistant.io/original/4X/1/a/1/1a129e306bc6a339cf8a2b9222553254a1909b6f.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/thetestspecimen/homeassistant/refs/heads/main/blueprints/ikea-bilresa-scroll-wheel.yaml)