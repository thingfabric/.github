# ThingFabric

**Matter in pure Go** — an embeddable library for the device and the controller
side, and the applications built on it. The stack implements the Matter
specification and follows [matter.js](https://github.com/matter-js/matter.js)
as its reference implementation: not a translation of its TypeScript, but its
behaviour, with parity held by tests.

| Repository | Import path | What it is |
| --- | --- | --- |
| [**go-fabric**](https://github.com/thingfabric/go-fabric) | `thingfabric.dev/go-fabric` | The library. Device side: TLV codec, Interaction Model, PASE/CASE, MRP over UDP and TCP, DNS-SD, the cluster servers and the endpoint assembler a bridge needs. Controller side: a full commissioner (BLE, Wi-Fi, Thread network steps) and controller. |
| [go-fabric-ui](https://github.com/SukramJ/go-fabric-ui) | `thingfabric.dev/go-fabric-ui` | One web interface for the daemons built on go-fabric: a Go module with the embedded bundle and a Svelte package. |
| [go-fabric-server](https://github.com/SukramJ/go-fabric-server) | `thingfabric.dev/go-fabric-server` | Controller server and bridge on go-fabric, over a WebSocket/JSON API compatible with Home Assistant's Matter integration. |
| [go-ha2fabric](https://github.com/SukramJ/go-ha2fabric) | `thingfabric.dev/go-ha2fabric` | Home Assistant entities as a bridge for Matter controllers. |

go-fabric lives here; the other three move over from `github.com/SukramJ`
one at a time, each together with its import path.

```sh
go get thingfabric.dev/go-fabric
```

📖 Documentation: **[docs.thingfabric.dev](https://docs.thingfabric.dev/)** ·
🌐 [thingfabric.dev](https://thingfabric.dev/) ·
All repositories are licensed under Apache-2.0.

### Not certified

These are independent open-source projects. They are **not certified by the
Connectivity Standards Alliance** and are not projects of the Alliance. Using
them does not make a device, product or service Matter certified or compliant.
"Matter" is a trademark of the Connectivity Standards Alliance.
