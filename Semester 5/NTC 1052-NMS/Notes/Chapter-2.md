# Chapter 2: Configuration Management (CM)

## What is CM???
- Process of recording, updating, and managing information about an organization's hardware and software. 
- Keep track of all devices, software versions, and updates applied across a network.

## How CM works?
> Network Devices >> Collect Data >> Store & Analyze >> Modify & Update Configurations >> Generate Reports

## What does CM involve ??
| Info | Description |
|------|-------------|
|**Gathering Information**| Collect details about current network configurations|
|**Modifying Configurations**| Update device settings when needed|
|**Storing Data**| Keep records of network components|
|**Maintaining Inventory**| Ensure all components are well documented|
|**Generating Reports**| Produce summaries based on stored data|

## Benefits of CM

1. Better Control Over Network Devices: 
    - Quickly access configuration data
    - Helps in troubleshooting and planning for future changes.

2. Easy Comparison and Modification
    - Can compare current settings with stored configurations and make necessary changes

3. Inventory Management
    - CM keeps up-to-date 
    - Stores important details like vendor contacts, leased-line numbers, etc
    > Security concern: If accessed by malicious individuals, this info could be used to harm the network.

## Steps in CM
1. Gather Network Information
2. Modify Device Configurations
3. Store and Maintain Inventory 

## Data Collection Methods
### Manual Collection
    Engineers log in to each device and record details in spreadsheets or databases

    Challenges: 
        - Time-consuming and error-prone
        - Difficult in large networks
        - May fail to detect new unauthorized devices

### Autodiscovery (Automated Collection)
    1. Query-Based Discovery (e.g ICMP Echo or Ping)
        Sends queries to all network devices

        Pro: Detects all active devices
        Con: Wastes bandwidth when querying non-existent devices

    2. Network Protocol Discovery
        Finds a know devices and queries, to detect other devices that communicated with

        Pro: Faster discovery
        Con: May miss inactive devices

## Data Modification & Storage
- Engineers can update device settings through CM tools
- Configurations are stored centrally for quick access

Storage Methods:
- ASCII Files : Simple, easy to read
- Database Management System (DBMS) : faster, structured storage 

## Configuration Management Tools
| Tools | Description |
|-------|-------------|
|**Simple Tools**|- Store data centrally <br> - Provide search and basic discovery futures|
|**Complex Tools**|- Automatically compare and update configurations <br> - Detect discrepnacies and suggest corrections|
|**Advanced Tools**|- Use DBMS to store and analyze network configurations <br> - Allow SQL queries to retrieve specific details|

### Real-World CM Tools
- ManageEngine Network Configuration Manager
- Kiwi CatTools
- SolarWinds Network Configuration Manager