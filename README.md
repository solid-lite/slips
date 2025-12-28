# Solid Lite Implementation Proposals (SLIPs)

SLIPs are composable building blocks for decentralized web servers. Pick the SLIPs you need — different combinations create different profiles.

## SLIP Index

### Core Foundation
| SLIP | Name | Status | JSS |
|------|------|--------|-----|
| [10](./10.md) | HTTP Methods | Draft | ✅ |
| [11](./11.md) | CORS Headers | Draft | ✅ |
| [12](./12.md) | JSON-LD | Draft | ✅ |
| 13 | URI Resources | Draft | ✅ |

### Identity
| SLIP | Name | Status | JSS |
|------|------|--------|-----|
| 20 | WebID Profile | Draft | ✅ |
| [21](./21.md) | did:nostr | Draft | ✅ |
| 22 | Identity Linking | Draft | ⏳ |

### Data & Formats
| SLIP | Name | Status | JSS |
|------|------|--------|-----|
| 30 | Turtle | Draft | ✅ |
| 31 | Content Negotiation | Draft | ✅ |
| 32 | Data Islands | Draft | ⏳ |
| 33 | PATCH | Draft | ✅ |

### Features
| SLIP | Name | Status | JSS |
|------|------|--------|-----|
| 40 | Containers | Draft | ✅ |
| 41 | Pods | Draft | ✅ |
| 42 | WebSockets | Draft | ✅ |
| 43 | Type Index | Draft | ⏳ |
| 44 | Mashlib/SolidOS | Draft | ✅ |

### Federation
| SLIP | Name | Status | JSS |
|------|------|--------|-----|
| 50 | ActivityPub | Draft | ⏳ |
| 51 | WebFinger | Draft | ⏳ |
| 52 | HTTP Signatures | Draft | ⏳ |
| 53 | Nostr Relays | Draft | ⏳ |

### Authentication
| SLIP | Name | Status | JSS |
|------|------|--------|-----|
| [80](./80.md) | Null Auth | Draft | ✅ |
| [81](./81.md) | Bearer Token | Draft | ✅ |
| [82](./82.md) | Schnorr/NIP-98 | Draft | ✅ |
| 83 | Solid-OIDC | Draft | ✅ |

### Authorization
| SLIP | Name | Status | JSS |
|------|------|--------|-----|
| [90](./90.md) | Owner Write | Draft | ✅ |
| 91 | WAC | Draft | ✅ |
| 92 | ACP | Draft | ⏳ |

## Profiles (Recipes)

Different SLIP combinations create different server profiles:

| Profile | SLIPs | Description |
|---------|-------|-------------|
| **Minimal** | 10, 11, 12, 80 | 10-minute implementation |
| **Single-User** | Minimal + 81, 90 | Personal data store |
| **LWS** | Core + 20, 83, 91, 40 | [W3C target](https://linkedwebstorage.com/) |
| **ActivityPub** | Minimal + 50, 51, 52 | [Fediverse](https://socialdocs.org/docs/ecosystem/fedbox/) |
| **Full JSS** | All SLIPs | Complete Solid server |
| **Nostr-Native** | Minimal + 21, 82, 91 | Passwordless, no registration |

## Contributing

1. **Discuss** your idea in GitHub Issues
2. **Draft** a SLIP following the template
3. **Submit** a Pull Request
4. **Review** and iterate with community
5. **Implement** in reference server (JSS)

## SLIP Numbering

- **1-99**: Core protocol
- **100-999**: Extended features
- **1000-9999**: Related projects
- **10000+**: Community extensions

## References

- [Solid Lite Spec](https://solid-lite.org)
- [JSS Reference Implementation](https://github.com/JavaScriptSolidServer/JavaScriptSolidServer)
- [Linked Web Storage (W3C)](https://linkedwebstorage.com/)
