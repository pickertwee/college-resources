# Chapter 3: SNMP

## SNMP (Simple Network Management Protocol)
Simplify the process by allowing uniform access to network devices from different manufactures.

## Network Management & Monitoring Process
Queries made to network devices can include:
- Software version
- Number of Interface
- Number of packets per second on an interface

### Management Information Base (MIB) 
- What information can be managed
- Contains hierarchical collection of objects -- each identified by a uniques Object Identifier (OID)

    Example of MIB Objects:
    - ifOutQLen (Output queue lenght)
    - atTable (Address Translation table)

### Structure of Management Information (SMI) 
- How information is structured 

SMI components:
1. Modules definitions: Organizes related objects
2. Object definitions: Describes individual data objects
3. Notification definitions: Defines event notifications (alerts)

## SNMP (Simple Network Management Protocol)
- Part of the Internet Protocol (IP) 
- Used to monitor network devices for administrative purposes

### SNMP Components
    1. Managed Devices
    2. Agents
    3. Network Management System (NMS)

### SNMP Functions
Operates at **Layer 7 (Application Layer)** OSI model

Uses five types of messages: 
- *get-request* : retrieve information
- *get-next* : retrieve next object
- *set-request* : modify a value 
- *get-response* : reply to request
- *trap* : send alerts

### SNMP Versions
 |Versions|Description|
 |--------|-----------|
 |**SNMPv1**| - Used five messages <br> - Weak security|
 |**SNMPv2**| - Improved performance and security <br> - GETBULK for retrieving large data <br> - Not widely adopted due to complexity|
 |**SNMPv3**| - Current standard with enhanced security features <br> 1. Message integrity <br> 2. Authentication <br> 3. Encryption |