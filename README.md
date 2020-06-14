# USharpSwitch
Dell Display Manager Switcher

Easily switch between workstations/laptops connected to the same Dell UltraSharp display via multiple inputs including multimonitor setups (DP 1.2 MST) 

Current batch of Dell screens have an issue where if you switch between DP/mDP, the main screen does not come out of powersave mode even if you reset the graphics card drivers. 

The issue is quite widespread and I haven't seen a FW fix yet but there's a workaround by forcing DDM (Dell Display Manager) to rescan on the target PC. For this, a P2P feature is involved until I can find a more practical way.

Currently uses DDM to facilitate DDC/CI communications with the monitor. 

Prerequisites: 

1.  Dell Display Manager
2. .NET Core 3.1 Runtime
