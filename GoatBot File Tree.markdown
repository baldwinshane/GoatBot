# GoatBot Repository File Tree

```plaintext
GoatBot/
├── README.md
├── LICENSE
├── docs/
│   ├── design_specification.md
│   ├── assembly_guide.md
│   ├── control_system_guide.md
│   ├── battery_management.md
│   ├── patent_workarounds.md
│   ├── material_selection.md
│   ├── testing_protocols.md
│   ├── navigation_guide.md
│   ├── thermal_management.md
├── cad/
│   ├── body/
│   │   ├── main_chassis.stl
│   │   ├── leg_mounts.stl
│   │   ├── cooling_duct.stl
│   ├── legs/
│   │   ├── upper_leg.stl
│   │   ├── lower_leg.stl
│   │   ├── hoof.stl
│   │   ├── suspension.stl
│   ├── head/
│   │   ├── pi_mount.stl
│   │   ├── screen_holder.stl
│   ├── fea/
│   │   ├── leg_stress_analysis.fea
│   │   ├── chassis_stress_analysis.fea
│   │   ├── suspension_stress_analysis.fea
├── src/
│   ├── control/
│   │   ├── main_control.py
│   │   ├── balance_controller.py
│   │   ├── terrain_adaptation.py
│   │   ├── motor_driver.py
│   │   ├── rl_model.py
│   │   ├── terrain_prediction.py
│   ├── interface/
│   │   ├── touchscreen_ui.py
│   │   ├── sensor_interface.py
│   ├── navigation/
│   │   ├── path_planning.py
│   │   ├── sensor_fusion.py
│   │   ├── gps_navigation.py
├── firmware/
│   ├── motor_firmware.ino
│   ├── bms_firmware.ino
│   ├── bldc_firmware.ino
├── bom/
│   ├── bill_of_materials.csv
│   ├── sourcing_guide.md
├── tests/
│   ├── unit_tests/
│   │   ├── test_balance.py
│   │   ├── test_terrain.py
│   │   ├── test_navigation.py
│   ├── integration_tests/
│   │   ├── test_full_system.py
├── scripts/
│   ├── setup_environment.sh
│   ├── flash_firmware.sh
├── configs/
│   ├── robot_config.yaml
│   ├── sensor_config.yaml
│   ├── navigation_config.yaml
└── media/
    ├── images/
    │   ├── robot_render.jpg
    │   ├── hoof_design.jpg
    │   ├── suspension_design.jpg
    ├── videos/
    │   ├── demo_walk.mp4
    │   ├── incline_test.mp4
    │   ├── high_speed_test.mp4
```

## File Descriptions (Updated)

- **README.md**: Updated with high-speed capabilities and return-home feature.
- **LICENSE**: BSD 3-clause, unchanged.
- **docs/**:
  - **design_specification.md**: Includes rPETG, BLDC motors, suspension, and AI terrain prediction.
  - **assembly_guide.md**: Adds suspension and cooling duct assembly steps.
  - **control_system_guide.md**: Details RL-based balance and AI terrain prediction.
  - **battery_management.md**: Covers 6S 8000mAh battery and regenerative braking.
  - **patent_workarounds.md**: Updated with BLDC motor and RTK navigation workarounds.
  - **material_selection.md**: Adds rPETG and recycled TPU details.
  - **testing_protocols.md**: Includes high-speed and navigation tests.
  - **navigation_guide.md**: New, describes GPS/RTK return-home system.
  - **thermal_management.md**: New, details cooling duct and fan system.
- **cad/**:
  - **body/**: Adds `cooling_duct.stl` for thermal management.
  - **legs/**: Adds `suspension.stl` for TPU-based suspension.
  - **fea/**: Adds `suspension_stress_analysis.fea`.
- **src/**:
  - **control/**: Adds `rl_model.py` for reinforcement learning, `terrain_prediction.py` for AI terrain analysis.
  - **navigation/**: Adds `gps_navigation.py` for return-home functionality.
- **firmware/**:
  - **bldc_firmware.ino**: New, controls BLDC motors.
- **bom/**:
  - **bill_of_materials.csv**: Adds BLDC motors, GPS module, LiDAR, cameras, fans.
  - **sourcing_guide.md**: Updated with refurbished component suppliers.
- **tests/**:
  - **unit_tests/**: Adds `test_navigation.py` for GPS/RTK tests.
  - **integration_tests/**: Updated `test_full_system.py` for high-speed stability.
- **configs/**:
  - **navigation_config.yaml**: New, for GPS/RTK settings.
- **media/**:
  - **images/**: Adds `suspension_design.jpg`.
  - **videos/**: Adds `high_speed_test.mp4`.