# Mohaned Hassan

Senior Software & Web Developer in the UK. I build tools for working with Earth Observation and geospatial data, and I'm building [Treebind](https://github.com/mohanedmoh/treebind), an open-source Kubernetes operator.

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohaned-hassan-60a483127/)
[![Medium](https://img.shields.io/badge/-Medium-12100E?style=flat-square&logo=medium&logoColor=white)](https://medium.com/@mohanedmoh)

## Treebind

[**Treebind**](https://github.com/mohanedmoh/treebind) keeps a Git repository and an application's files in sync, in both directions, through a shared Kubernetes volume. You declare a `Treebind` resource that names the repository, an existing PVC and the sync policy. The operator runs a sync agent that pulls remote changes, commits the application's own edits and can push them back. The application can be any program that reads and writes those files: a dashboard tool, a workflow engine, a website.

- **Stack:** Go, kubebuilder and controller-runtime. Apache-2.0.
- **First release (M1):** file-level sync.
- **Conflicts:** designed to be set per resource. The default follows the remote and keeps local work on a side branch; the alternative follows local.
- **Next:** adapters for tools such as Grafana, which export their data to files and sync those.
- **Storage:** built for single-node clusters first (k3s, kind), with the design left open for Ceph, NFS, managed cloud Kubernetes and multi-node clusters.
- **Status:** early alpha, not ready for real data yet. The first working release is tracked in the [M1 MVP milestone](https://github.com/mohanedmoh/treebind/milestones), and the issues are open for contributors.

The name: "tree" is Git's working tree, and "bind" is binding that tree to a volume and keeping the two in step.

## Open source

Merged:

- [eodag](https://github.com/CS-SI/eodag/pull/2383): added an `eodag queryables` CLI command to inspect search parameters per provider and collection
- [stac-fastapi](https://github.com/stac-utils/stac-fastapi/pull/991): fixed Python-version-dependent error messages for out-of-range datetimes

In review:

- [geodiff](https://github.com/MerginMaps/geodiff/pull/266): added a schema comparison API (`GEODIFF_hasEqualSchema`) to check whether two data sources have the same table schemas without creating a changeset

## Skills

- **Cloud native:** Kubernetes operators and CRDs, Docker, infrastructure administration
- **Backend and web:** Go, Python, Laravel, Vue.js, Android
- **Geospatial and EO:** GeoServer (wrote a plugin), STAC, eodag
- **Graph databases:** Neo4j (certified)

## Writing

My MSc research was on graph databases. I publish articles on [Medium](https://medium.com/@mohanedmoh).

**Graph databases and algorithms** (from my MSc research)

- [Part 3: Build Your Own Graph Algorithm](https://mohanedmoh.medium.com/part-3-build-your-own-graph-algorithm-eddd3f5b603b) (Nov 2026)
- [Part 2: Run Graph Algorithms and See How They Work](https://mohanedmoh.medium.com/part-2-run-graph-algorithms-and-see-how-they-work-bfe65c7186b1) (Nov 2026)
- [Part 1: Set Up Your First Graph Database](https://mohanedmoh.medium.com/part-1-set-up-your-first-graph-database-c9a0499ed894) (Nov 2026)

**Earth Observation**

- [Why satellite AI still needs people on the ground](https://mohanedmoh.medium.com/why-satellite-ai-still-needs-people-on-the-ground-ccdc2a4bd302) (Oct 2026)

**VMware NSX-T** (2022)

- [NSX-T: Network Address Translation Configuration](https://mohanedmoh.medium.com/configuring-nat-in-nsx-t-c5625606f930)
- [NSX-T Load Balancer Configuration](https://mohanedmoh.medium.com/nsx-t-load-balancer-configuration-22b426653451)
- [Deploying NSX-T using VMware Workstation](https://mohanedmoh.medium.com/deploying-nsx-t-by-using-vmware-workstation-from-scratch-7b5da1213f91)
- [Workaround to Solve Edge Nodes Unsupported AMD CPUs](https://mohanedmoh.medium.com/workaround-to-solve-edge-nodes-unsupported-amd-cpus-1b2ebb0ef49d)
- [NSX-T 3.2 Transport Node Preparation Failed](https://mohanedmoh.medium.com/nsx-t-3-2-transport-node-preparation-failed-e3bf3135869)
