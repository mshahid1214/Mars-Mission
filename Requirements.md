
#Functional Requirements (FRs)

###FR-01 (Command Execution): 
The rover shall receive and execute valid movement and operational commands from Mission Control.

###FR-02 (Telemetry Reporting): 
The rover shall transmit location data, battery level, temperature, and communication status to Mission Control.

###FR-03 (Command Authentication & Validation):
The system shall verify operator credentials and reject invalid or unauthorized commands.

###FR-04 (Automated Safe Mode): 
The rover shall automatically transition into a Safe Mode state upon detecting a critical fault (e.g., severe thermal or battery conditions).

###FR-05 (Audit Logging): 
The system shall log all issued commands and critical rover events alongside timestamps and operator IDs for post-mission investigation.

###FR-06 (Command Status Feedback): 
Mission Control shall receive confirmation and execution status updates for each command sent to the rover.

#Non-Functional Requirements (NFRs)

###NFR-01 (Performance / Latency): 
Command processing shall complete within 5 seconds after the command is received by the rover.

###NFR-02 (Security):
The system shall restrict command issuance exclusively to authenticated Mission Control operators.

###NFR-03 (Reliability / Fault Tolerance):
The system shall maintain core operations and handle temporary communication dropouts caused by signal delay or atmospheric interference without loss of state.

###NFR-04 (Scalability): 
The system shall support simultaneous communication links and data handling across multiple active rovers.
