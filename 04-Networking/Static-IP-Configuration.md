## Final Configuration

| Setting | Value |
|---------|-------|
| IP Address | 192.168.56.10 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | None (Host-Only Network) |
| Preferred DNS | 192.168.56.10 |
| Alternate DNS | None |

## Why This Configuration?

The server is being prepared for Active Directory Domain Services (AD DS).

A static IP address ensures the Domain Controller always has a consistent network identity.

The server is configured to use itself as its preferred DNS server because it will later host the DNS service required by Active Directory.
