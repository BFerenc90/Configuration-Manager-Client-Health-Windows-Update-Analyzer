# Configuration Manager Client Health & Windows Update Analyzer

PowerShell-based diagnostic and reporting tool for Microsoft Configuration Manager (ConfigMgr / MECM / MCM / SCCM) clients.

Sample report: [View Interactive Sample Report](https://BFerenc90.github.io/Configuration-Manager-Client-Health-Windows-Update-Analyzer/CLIENT1_ConfigMgr_TS_Report.html)

# Overview

This script performs a comprehensive health assessment of a Configuration Manager client and generates a detailed troubleshooting report. It collects client configuration data, Windows Update settings, inventory information, networking details, and relevant log files, then analyzes the collected data against a large set of validation checks.

# The Goal

The goal is to quickly identify common client-side issues that may affect:

- Software Update deployments
- Client policy processing
- Content download and distribution
- Client registration and communication
- Hardware inventory
- Client health status
- Windows Update integration
- Management and Distribution Point communication
- Features
- Data Collection

The script automatically collects information from multiple sources, including:

- Configuration Manager client configuration
- Windows Update policies
- Delivery Optimization settings
- Antivirus products
- Azure AD (EntraID) / Hybrid Join status (dsregcmd)
- Group Policy results
- Installed and missing updates
- DISM packages and capabilities
- Windows features
- Hardware inventory
- Network configuration
- Automated Health Checks

# Configuration Manager Functionality & Health Checks

More than 60 validation checks are performed, including:

- Client installation validation
- Site assignment verification
- Maintenance window configuration
- WSUS configuration and connectivity
- Management Point connectivity
- Certificate validation
- BITS transfer monitoring
- Client settings verification
- Pending reboot detection
- Provisioning mode validation
- Disk space checks
- DNS resolution tests
- SCCM service health validation
- Policy processing verification
- Software Update scan and deployment validation
- WMI namespace and repository checks
- Client messaging validation
- Hardware inventory status
- Client Health (CcmEval) analysis
- Log Analysis
- etc...

The report contains recommended remediation actions and details if a check fails.

# Log Analyzes 

The tool automatically extracts and analyzes key Configuration Manager log files, including:

- ClientIDManagerStartup.log
- ClientLocation.log
- LocationServices.log
- PolicyAgent.log
- CcmMessaging.log
- CcmEval.log
- CcmExec.log
- ExecMgr.log
- InventoryAgent.log
- WUAHandler.log
- UpdatesDeployment.log
- UpdatesHandler.log
- UpdatesStore.log
- ScanAgent.log
- CAS.log
- ContentTransferManager.log
- DeltaDownload.log
- DataTransferService.log

The analyzer highlights relevant warning and error entries to reduce troubleshooting time.

# License

This project is licensed under the MIT License.
