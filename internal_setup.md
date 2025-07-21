# Internal Setup

- **Covered RPi** (external, labeled)
- **Uncovered RPi** (inside the robot)

### Snoopy Controller + Charlie Brown RPi
1. SSH:
   - Covered (external): `ssh ubuntu@192.168.2.32`
   - Uncovered (in robot): `ssh ubuntu@192.168.2.30`
2. Covered RPi:
   - `bluetoothctl`
   - `connect E4:17:D8:8C:5A:0F` (8BitDo Lite 2)
   - `quit`
   - `./start_controller.sh` (after calibrating)
3. Uncovered RPi:
   - Calibrate with ODrive
   - `./start_mobile_base.sh`

### Woodstock Controller + Peanuts RPi
1. SSH:
   - Covered (external): `ssh ubuntu@192.168.2.29`
   - Uncovered (in robot): `ssh ubuntu@192.168.2.53`
2. Covered RPi:
   - `bluetoothctl`
   - `connect E4:17:D8:4C:F5:84` (8BitDo Lite 2)
   - `quit`
   - `./start_controller.sh` (after calibrating)
3. Uncovered RPi:
   - Calibrate with ODrive
   - `./start_mobile_base.sh`
