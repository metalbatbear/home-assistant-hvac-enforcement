# home-assistant-hvac-enforcement
Sync mode and setpoints between multiple thermostats for combined-return HVAC systems

For quasi-multizone central HVAC systems (i.e., with a combined return), it may be necessary to keep all the thermostats synced to the same mode (heat, cool, off, etc.) and within a small temperature differential of each other (about 1.11°C or 2°F is typically the maximum permitted differential).  These automations sync the other thermostats to any thermostat that initiates a change.  (There is a small delay before syncing the changes to allow user input to settle and to prevent runaway changes.)

* hvac_mode_enforcement-automation.yaml runs by itself
* hvac_temperature_enforcement-automation.yaml calls hvac_temperature_enforcement-script.yaml
