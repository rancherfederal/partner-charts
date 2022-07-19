# Platform One's BigBang

Big Bang is a declarative, continuous delivery tool for core DoD hardened and approved packages into a Kubernetes cluster.

> _This is a mirror of a government repo hosted on [Repo1](https://repo1.dso.mil/) by [DoD Platform One](http://p1.dso.mil/).  Please direct all code changes, issues and comments to https://repo1.dso.mil/platform-one/big-bang/bigbang_

## Chart Details

This chart is built on the foundation of [Iron Bank](https://ironbank.dso.mil/) containers, and serves as the reference deployment for the DoD DevSecOps Reference architecture.

It uses gitops with [flux v2](https://fluxcd.io/docs/) to declaratively deploy and orchestrate the following core capabilities:

* Service Mesh (Istio, Kiali, Jaeger)
* Logging (EFK)
* Monitoring (Prometheus + Grafana)
* Policy Enforcement (OPA Gatekeeper)
* Cluster Auditing
* Runtime Defense (Twistlock)
