# Ticket 06 – DNS Resolution Failure

## Issue
User reported that internet connectivity appeared functional but websites could not be accessed.

## Environment
- Windows 11 Virtual Machine
- Hosted using UTM on macOS

## Initial Symptoms
- Ping to external IP address successful
- Domain names failed to resolve

Example tests performed:

ping 8.8.8.8
ping google.com

Results:
- 8.8.8.8 responded successfully
- google.com failed to resolve

## Troubleshooting Steps

1. Verified internet connectivity using:

ping 8.8.8.8

Result confirmed the system had network access.

2. Tested DNS resolution using:

ping google.com

Result indicated DNS resolution failure.

3. Investigated potential DNS configuration issues.

4. Discovered incorrect entry in the system hosts file redirecting the domain.

5. Removed the incorrect hosts file entry.

6. Cleared DNS cache using:

ipconfig /flushdns

## Resolution
Removed incorrect hosts file entry and cleared DNS cache, restoring proper DNS resolution.

## Verification
Successfully resolved domain name after correction:

ping google.com

## Skills Demonstrated
- DNS troubleshooting
- Command line diagnostics
- Windows network configuration
- System configuration analysis
