# Project Documentation: Active Directory Home Lab

## Introduction
The Active Directory, Splunk, and Kali Linux Home Lab project has undergone significant enhancements to simulate a comprehensive environment for system administration, log management, and security testing. This documentation provides a detailed account of the updated setup, including the integration of a healthcare organization, "Cryptic Clinic," into the existing domain infrastructure.

## Objectives
- Establish a virtualized environment using VirtualBox.
- Configure VMs including Windows 10, Kali Linux, Windows Server 2022 (Active Directory), and Ubuntu Server with Splunk.
- Enhance logging and monitoring capabilities through Sysmon and Splunk.
- Extend the domain environment to encompass the infrastructure of "Cryptic Clinic" adhering to the Australian Protective Security Policy Framework (PSPF).
- Implement security measures, including Group Policy Objects (GPOs) and account lockout policies.
- Conduct ethical hacking exercises, including a brute force attack, and monitor telemetry via Splunk.

## Setup
1. **Logical Diagram:**
   - Utilizing Draw.io, a logical diagram was created to visualize the architecture of the home lab environment. The diagram illustrates the network configuration, including IP addresses and connectivity between VMs, Splunk server, Active Directory, and the internet.

2. **Installing VMs:**
   - VirtualBox was utilized to deploy the following VMs:
     - Windows 10
     - Kali Linux
     - Windows Server 2022 (Active Directory)
     - Ubuntu Server with Splunk

## Installation and Configuration
1. **Sysmon & Splunk Configuration:**
   - Sysmon and Splunk were installed and configured on Windows 10 and Windows Server to enhance logging and monitoring capabilities.

2. **Active Directory Configuration:**
   - Windows Server 2022 was deployed and configured as the primary domain controller.
   - Organizational Units (OUs) were created for "Cryptic Clinic" and its departments within Active Directory.
   - User accounts were created for individuals within "Cryptic Clinic."

3. **Group Policy Object (GPO) Creation:**
   - A new GPO named "Cryptic Clinic Policies" was created within Active Directory for enforcing security policies.
   - Security settings, including password policies and Windows Firewall rules, were configured to align with the Australian PSPF.

4. **Account Lockout Policies:**
   - Account lockout policies were implemented to mitigate brute force attacks:
     - Account lockout duration: 15 minutes
     - Account lockout threshold: 5 attempts
     - Admin account lockout: Disabled
     - Reset account lockout counter after: 15 minutes

## Integration of "Cryptic Clinic"
- "Cryptic Clinic" was integrated into the existing domain environment by creating dedicated OUs for the medical and administrative departments.
- User accounts were provisioned for individuals within "Cryptic Clinic," including practitioners, support staff, and system administrators.

## Ethical Hacking and Telemetry Monitoring
- Ethical hacking exercises, such as a brute force attack using Kali Linux, were conducted to assess security posture.
- Splunk was utilized to monitor telemetry and analyze security events, providing insights into potential security incidents.

## Conclusion
The updated Active Directory Home Lab project, now incorporating "Cryptic Clinic," offers an immersive learning experience in system administration, log management, and ethical hacking within a simulated healthcare organization environment. By adhering to security best practices and leveraging advanced tools like Splunk and Atomic Red Team, participants gain practical skills applicable to real-world IT scenarios and security practices.

## Future Considerations
- Further exploration of security frameworks such as MITRE and ATT&CK.
- Continuous updates and expansions to the home lab environment to simulate evolving security threats.
- Collaboration with peers and contributions to the cybersecurity community to share insights and best practices.
