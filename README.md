# core-UWLab (Custom grblHAL Core)

## Overview
This is a modified fork of the grblHAL core, designed to support a 2-axis CNC plasma cutting system for the ME 481/482 capstone project at the University of Waterloo. The modifications improve safety by adjusting Feed Hold behavior to stop the spindle (torch) as well, even when not in laser mode.

## Key Modifications
- **Feed Hold Behavior**: 
  - Modified so that activating Feed Hold stops the spindle (torch), not just the motion.
  - Previously, spindle stop was only enforced in laser mode.
- **Integration with STM32F4xx Fork**:
  - Used in a custom fork of `grblHAL/STM32F4xx` (UWLab version) to match our machine’s requirements.

## Date
March 12, 2025
