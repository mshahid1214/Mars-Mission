
#Functional Requirements (FRs)

###FR-01 
The rover shall receive and execute valid movement and operational commands from Mission Control.

###FR-02 
The rover shall transmit location data, battery level, temperature, and communication status to Mission Control.

###FR-03 (Command Authentication & Validation):
The system shall verify operator credentials and reject invalid or unauthorized commands.

###FR-04:
The rover shall enter Safe Mode within 3 seconds whenbattery temperature exceeds the critical threshold/battery capacity. 
###FR-05 
The system shall log all issued commands and critical rover events alongside timestamps and operator IDs for post-mission investigation.

###FR-06
Mission Control shall receive confirmation and execution status updates for each command sent to the rover.

#Non-Functional Requirements (NFRs)

###NFR-01
Command processing shall complete within 5 seconds after the command is received by the rover.

###NFR-02 
The system shall restrict command issuance exclusively to authenticated Mission Control operators.

###NFR-03 
The system shall maintain core operations and handle temporary communication dropouts caused by signal delay or atmospheric interference without loss of state.

###NFR-04
The system shall support simultaneous communication links and data handling across multiple active rovers.
