# USharpSwitch
Dell Display Manager Switcher

"Fake" KVM without the actual k/m part (for now).

Easily switch between workstations/laptops connected to same Dell UltraSharp display with multiple inputs including multimonitor setups via DP 1.2 MST (laptop+PC connected to main screen, secondary daisy-chained to primary via DP MST)

Current batch of Dell screens have an issue where if you switch between DP/mDP, the main screen does not come out of powersave mode even if you reset the graphics card drivers. 

The issue is quite widespread and I haven't seen a FW fix yet but there's a workaround by forcing DDM (Dell Display Manager) to rescan on the target PC. For this, some client/server solution is involved until I can find a easier way.

Currently uses DDM to facilitate DDC/CI communications with the monitor. 

Prerequisites: 

1. Dell Display Manager
2. .NET Core 3.1 Runtime
