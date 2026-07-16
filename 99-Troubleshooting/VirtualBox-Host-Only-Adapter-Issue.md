# VirtualBox Host-Only Adapter Issue

## Problem

VirtualBox failed to start TS-DC01 with the error:

VERR_INTNET_FLT_IF_NOT_FOUND

## Investigation

- Verified VM adapter configuration.
- Confirmed Host-only Adapter existed in VirtualBox.
- Confirmed Windows detected the VirtualBox Host-Only Ethernet Adapter.
- Attempting to refresh the adapter binding.

## Outcome

The issue was resolved by refreshing the VirtualBox Host-Only Adapter.

### Steps Taken

1. Opened Windows Network Connections (`ncpa.cpl`).
2. Verified that the VirtualBox Host-Only Ethernet Adapter existed.
3. Disabled the adapter.
4. Waited approximately 10 seconds.
5. Re-enabled the adapter.
6. Restarted the virtual machine.

### Result

The virtual machine started successfully without further errors.

### Lesson Learned

When VirtualBox reports `VERR_INTNET_FLT_IF_NOT_FOUND`, verify the Host-Only Adapter before reinstalling VirtualBox. Refreshing the adapter binding may resolve the issue.
