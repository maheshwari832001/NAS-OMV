# Deploying a NAS Server Using OpenMediaVault
This project demonstrates the setup of a Network Attached Storage (NAS) system using OpenMediaVault in VirtualBox.

## Objective
- To deploy a NAS server using OMV, enabling centralized file storage, sharing, and management over a network.

## Tools Used
- Oracle VirtualBox
- OpenMediaVault 7.4.17
- SMB/CIFS Protocol
- EXT4 File System
- Windows File Access

## Folder Structure

- `home`: Personal folders
- `privateshare`: Restricted shared folder
- `publicshare`: Public read-only folder

## Users & Groups
- Users: maheshwari, swathi, swagath
- Groups: team1, team2, team3

## Access Summary
| Folder       | Access Type             | Who Has Access                         |
|--------------|-------------------------|----------------------------------------|
| home         | Private Read/Write      | Each user to their own folder          |
| privateshare | Restricted Read/Write   | Only specific users                    |
| publicshare  | Guest Read-Only         | Everyone     (No credentials required) |       


## Troubleshooting
- Faced SMB permission issues
- Resolved via user groups and folder permission settings
- Faced `502 Bad Gateway` Error in OpenMediaVault Web UI After System Update
- Refer to: `Fixing 502 error.pdf`


## Conclusion
Successfully deployed a fully functional NAS in VirtualBox, configured file sharing protocols, tested access from multiple devices, and documented the entire process.
