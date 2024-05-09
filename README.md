# lbr_fri_msgs
Interface definition language (IDL) messages for the FRI.

## Command Interfaces
- [LBRPositionCommand.msg](msg/LBRPositionCommand.msg):
    - Client command mode: `Position`
    - Joint position
- [LBRTorqueCommand.msg](msg/LBRTorqueCommand.msg): 
    - Client command mode: `Torque`
    - Joint position and torque overlay commands
- [LBRWrenchCommand.msg](msg/LBRWrenchCommand.msg): 
    - Client command mode `Wrench`
    - Joint position and wrench overlay commands

- [LBRCommand.msg](msg/LBRCommand.msg):
    - Combined message to buffer the above

## State Interfaces
- [LBRState.msg](msg/LBRState.msg):
    - FRI exposed robot state
