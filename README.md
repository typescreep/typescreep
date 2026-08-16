<div align="center">

# typescreep

### I turn YAML into interfaces people can actually use.

`TypeScript` · `React` · `Node.js` · `Kubernetes` · `OpenAPI`

**STATUS: AVAILABLE FOR HIRE**

</div>

---

```yaml
developer:
  handle: typescreep
  specialty: making complicated infrastructure feel less complicated
  current_mission:
    - discover Kubernetes resources
    - understand their schemas
    - generate useful interfaces
    - keep everything live over WebSockets
  fuel: coffee
  availability: open to full-time and contract work
```

Most interfaces begin with a designer and a collection of screens.

Mine can begin with a Kubernetes Custom Resource Definition.

I build systems that inspect schemas, understand resources, and assemble the tables, forms, dashboards, terminals, navigation, and data flows needed to operate them. The result is not another hardcoded admin panel — it is a UI platform that adapts to the infrastructure behind it.

My main work lives across three repositories:

```text
                         ┌──────────────────────────┐
                         │       openapi-ui         │
                         │   the working console    │
                         └────────────┬─────────────┘
                                      │ consumes
                         ┌────────────▼─────────────┐
                         │   openapi-k8s-toolkit    │
                         │ components + factories  │
                         └────────────┬─────────────┘
                                      │ talks through
                         ┌────────────▼─────────────┐
                         │   openapi-ui-k8s-bff     │
                         │ Kubernetes + OpenAPI BFF │
                         └────────────┬─────────────┘
                                      │
                         ┌────────────▼─────────────┐
                         │        Kubernetes        │
                         └──────────────────────────┘
```

### The console

[PRO-Robotech/openapi-ui](https://github.com/PRO-Robotech/openapi-ui) is a React application that discovers CRDs, watches their objects, and renders a live interface from declarative configuration. It includes plugin-powered navigation, theming, terminals, graphs, generated forms, and resource views.

### The engine room

[PRO-Robotech/openapi-k8s-toolkit](https://github.com/PRO-Robotech/openapi-k8s-toolkit) contains the reusable machinery: schema-driven forms, Kubernetes-aware tables, smart query hooks, logs, terminals, dashboards, and a factory engine that resolves JSON or YAML into working React components.

### The bridge

[PRO-Robotech/openapi-ui-k8s-bff](https://github.com/PRO-Robotech/openapi-ui-k8s-bff) handles the less visible work between browser and cluster: API and WebSocket proxying, impersonation, OpenAPI schema caching, customization, metrics, health checks, and safe log filtering.

---

I like problems where frontend architecture meets infrastructure — especially when the answer is a reusable system instead of the fifteenth slightly different CRUD screen.

Things I care about:

- declarative systems that remain understandable
- real-time interfaces that behave predictably
- abstractions that remove work instead of relocating it
- tools that respect both their users and their maintainers
- strong TypeScript boundaries around messy external APIs

Things I use along the way:

`React` `Redux Toolkit` `TanStack Query` `Ant Design` `Storybook` `Express` `WebSockets` `Prometheus` `Jest` `Docker` `Helm`

---

<div align="center">

### Have an interesting platform problem?

I'm available for **full-time roles** and **contract work** involving TypeScript, frontend systems, Node.js, Kubernetes, OpenAPI, internal platforms, or developer tooling.

[Open a conversation](https://github.com/typescreep) — coffee optional, interesting problem required.

</div>
