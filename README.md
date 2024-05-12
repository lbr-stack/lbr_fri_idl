# lbr_fri_idl
Interface definition language (IDL) messages for the FRI.

## Command Interfaces
- `LBRPositionCommand.msg`:
    - Control modes:
        - `POSITION_CONTROL`
        - `JOINT_IMPEDANCE_CONTROL`
        - `CARTESIAN_IMPEDANCE_CONTROL`
    - Client command mode: `Position`
    - Contains:
        - Joint position
- `LBRTorqueCommand.msg`:
    - Control mode: `JOINT_IMPEDANCE_CONTROL`
    - Client command mode: `Torque`
    - Contains:
        - Joint position and torque overlay commands
- `LBRWrenchCommand.msg`: 
    - Control mode: `CARTESIAN_IMPEDANCE_CONTROL`
    - Client command mode: `Wrench`
    - Contains:
        - Joint position and wrench overlay commands

- `LBRCommand.msg`:
    - Combined message to buffer the above

## State Interfaces
- `LBRState.msg`:
    - FRI exposed robot state
