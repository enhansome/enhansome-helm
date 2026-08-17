# Awesome Helm with stars

> A collaborative list of awesome [Helm](https://helm.sh) resources.

Helm is the package manager for Kubernetes, it makes deploying complex application workloads simple, helps organize the update process.

# Contents

<!-- TOC -->

* [Guides](#guides)
* [Repositories / hubs](#repositories--hubs)
* [Application repositories](#application-repositories)
* [Plugins](#plugins)
* [Tools, Extras](#tools-extras)
* [Testing](#testing)
* [Community](#community)

## Guides

* [How to create your first helm chart](https://techdocs.broadcom.com/us/en/vmware-tanzu/application-catalog/tanzu-application-catalog/services/tac-doc/apps-tutorials-create-first-helm-chart-index.html) - Broadcom guide on authoring your first chart
* [Authoring awesome charts](https://github.com/helm/helm-classic/blob/master/docs/awesome.md) ⚠️ Archived - official Helm guide on authoring Awesome Charts
* [Kompose](https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/) - how to translate a docker-compose file into a Helm chart

## Repositories / hubs

Official Kubernetes Helm repositories

* [Kubernetes Helm charts stable repo](https://github.com/helm/charts/tree/master/stable) ⚠️ Archived
* [Kubernetes Helm charts incubating repo](https://github.com/helm/charts/tree/master/incubator) ⚠️ Archived
* [Helm Hub](https://hub.helm.sh) - Official Helm Hub

3rd party repositories / hubs

* [Cloudsmith](https://cloudsmith.io/l/helm-repository/) - A fully managed package management SaaS, with first-class support for public and private Kubernetes registries (Docker + Helm Charts, plus many others). Has a generous free-tier and is also completely free for open-source.
* [Fabric8](https://fabric8.io/helm/) - chart repository by Fabric8
* [Kubeapps](https://hub.kubeapps.com/) - Kubeapps helm chart hub by Bitnami
* [Fairwinds](https://hub.helm.sh/charts/fairwinds-stable) - Chart hub by Fairwinds
* [ChartCenter](https://chartcenter.io) - Central repository of Helm charts by JFrog
* [Meshery Catalog](https://meshery.io/catalog) - Well-architected patterns for Kubernetes and all CNCF projects

## Application repositories

These usually hold a single chart or a group of connected charts. Can be more up to date than the mainstream Kubernetes repos.

* [Zalenium](https://github.com/zalando/zalenium/tree/master/charts/zalenium) ⚠️ Archived - flexible and scalable container based Selenium Grid with video recording, live preview, basic auth & dashboard
* [Elastic](https://github.com/elastic/helm-charts/) ⚠️ Archived - Official helm charts for [Elatic.co](https://www.elastic.co/)'s open source products (ElasticSearch, Kibana & filebeat)
* [Harbor](https://github.com/goharbor/harbor-helm) ⭐ 1,509 | 🐛 73 | 🌐 Mustache | 📅 2026-08-03 - Harbor is a container and Helm registry with built-in security
* [OpenStack](https://github.com/openstack/openstack-helm) ⭐ 573 | 🐛 0 | 🌐 Shell | 📅 2026-08-13 - various charts by the OpenStack project
* [Mocktail](https://github.com/Huseyinnurbaki/mocktail) ⭐ 270 | 🐛 20 | 🌐 TypeScript | 📅 2026-08-15 - Helm chart for deploying the free, tiny mock api server Mocktail
* [KubeStellar Console](https://github.com/kubestellar/console) ⭐ 128 | 🐛 28 | 🌐 TypeScript | 📅 2026-08-17 - AI-powered multi-cluster Kubernetes management console with built-in Helm chart for one-command deployment
* [Bitwarden](https://github.com/cdwv/bitwarden-k8s) ⭐ 96 | 🐛 6 | 🌐 Mustache | 📅 2025-01-23 - Helm chart for deploying bitwarden-rs - unofficial Bitwarden-compatible server
* [Lenses](https://github.com/Landoop/kafka-helm-charts) ⚠️ Archived - charts for Lenses, Apache Kafka, Kafka Connect and other components for data streaming and data integration
* [Fn Project](https://github.com/fnproject/fn-helm) ⭐ 59 | 🐛 10 | 🌐 Smarty | 📅 2019-03-20 - Fn serverless platform charts
* [Elasticsearch Fluentd Kibana](https://github.com/cdwv/efk-stack-helm) ⭐ 57 | 🐛 4 | 🌐 Smarty | 📅 2020-09-19 - chart to deploy a full EFK stack for Kubernetes monitoring
* [Gitlab Omnibus](https://charts.gitlab.io) - an All-In-One chart for deploying Gitlab in Kubernetes
* [Jupyterhub and Binderhub](https://jupyterhub.github.io/helm-chart/) - charts for deploying services to run Jupyter notebooks
* [Ingero](https://github.com/ingero-io/ingero) - eBPF-based GPU causal observability agent. Helm chart deploys as DaemonSet with RBAC, traces CUDA APIs and host kernel events to explain GPU latency.

## Plugins

* [Helm Diff](https://github.com/databus23/helm-diff) ⭐ 3,480 | 🐛 54 | 🌐 Go | 📅 2026-08-17 - Plugin that shows a diff explaing what a `helm upgrade` and `helm rollback` would change. It can also compare two separate revisions of the release.
* [Helm Secrets](https://github.com/jkroepke/helm-secrets) ⭐ 2,024 | 🐛 1 | 🌐 Shell | 📅 2026-08-14 - Plugin to manage and store secrets safely.
* [Helm Unittest](https://github.com/helm-unittest/helm-unittest) ⭐ 1,383 | 🐛 78 | 🌐 Go | 📅 2026-08-03 - Plugin that enables you to run BDD style unit tests against rendered Helm charts. Adds the `helm unittest` command to execute tests.
* [Helm S3](https://github.com/hypnoglow/helm-s3) ⭐ 614 | 🐛 40 | 🌐 Go | 📅 2026-08-02 - Plugin to fetch charts from S3.
* [Helm Monitor](https://github.com/ContainerSolutions/helm-monitor) ⭐ 420 | 🐛 13 | 🌐 Go | 📅 2023-09-05 - Plugin to monitor a release and rollback based on Prometheus/ElasticSearch query.
* [Helm GCS](https://github.com/hayorov/helm-gcs) ⭐ 284 | 🐛 8 | 🌐 Go | 📅 2026-08-13 - Plugin that manages chart repos on Google Cloud Storage privately.
* [Helm Schema](https://github.com/dadav/helm-schema) ⭐ 280 | 🐛 11 | 🌐 Go | 📅 2026-08-17 - Auto-generate jsonschema files for helm charts.
* [Helm Compose](https://github.com/seacrew/helm-compose) ⚠️ Archived - Plugin that allows coupled multi release handling of one or many charts. With full configuration-as-code capabilities in a single yaml file similar to docker-compose.
* [Helm Schema Gen](https://github.com/karuppiah7890/helm-schema-gen) ⚠️ Archived - So that you don't have to write `values.schema.json` by hand from scratch for your Helm 3 charts
* [Helm Cel](https://github.com/idsulik/helm-cel) ⭐ 134 | 🐛 0 | 🌐 Go | 📅 2025-10-21 - Plugin that uses Common Expression Language ([CEL](https://cel.dev/)) to validate values.
* [Helm Datree](https://github.com/datreeio/helm-datree) ⭐ 117 | 🐛 2 | 🌐 Shell | 📅 2024-06-20 - Plugin to prevent Kubernetes misconfigurations by ensuring that Helm charts follow best practices as well as your organization’s policies
* [Helm Release](https://github.com/JovianX/helm-release-plugin) ⭐ 111 | 🐛 12 | 🌐 Shell | 📅 2026-03-29 - Plugin that pulls(re-creates) Helm charts from deployed releases, also allows update values of deployed releases without supplying the chart(for modified or custom charts, or when there's no access to the chart)
* [Helm Dt](https://github.com/vmware-labs/distribution-tooling-for-helm) ⭐ 108 | 🐛 11 | 🌐 Go | 📅 2026-07-22 - Plugin that helps moving Helm charts across OCI registries.
* [Helm Teller](https://github.com/SpectralOps/helm-teller) ⭐ 69 | 🐛 1 | 🌐 Go | 📅 2022-11-14 - Plugin that allows you to manage deployment configuration and secrets from multiple providers securely with [Teller](https://github.com/SpectralOps/teller) ⭐ 3,227 | 🐛 51 | 🌐 Rust | 📅 2026-01-27
* [Helm Starter](https://github.com/salesforce/helm-starter) ⭐ 63 | 🐛 4 | 🌐 Shell | 📅 2026-06-02 - Plugin that simplifies working with helm chart starter packs.
* [Helm Kanvas Snapshot](https://github.com/meshery/helm-kanvas-snapshot) ⭐ 45 | 🐛 13 | 🌐 Go | 📅 2026-08-06 - Plugin that generates a visual snapshot of Helm charts.
* [Helm Local](https://github.com/adamreese/helm-local) ⭐ 23 | 🐛 0 | 🌐 Shell | 📅 2018-09-11 - Plugin to run Tiller (helm 2's server-side component) as a local daemon.
* [Helm Env](https://github.com/adamreese/helm-env) ⭐ 22 | 🐛 1 | 🌐 Shell | 📅 2022-01-19 - Plugin to show the environment variables available to a helm plugin.
* [Helm Nuke](https://github.com/adamreese/helm-nuke) ⭐ 19 | 🐛 0 | 🌐 Shell | 📅 2018-02-27 - Plugin that deletes and purges all releases stored by Tiller.
* [Helm GitHub](https://github.com/web-seven/helm-github) ⭐ 14 | 🐛 1 | 🌐 JavaScript | 📅 2023-07-25 - Plugin that detects and install Helm Charts from GitHub Public/Private Repository Releases.
* [Helm Last](https://github.com/adamreese/helm-last) ⭐ 13 | 🐛 1 | 🌐 Makefile | 📅 2018-08-02 - Plugin that shows the latest release interacted with. This is useful for chaining commands together like `helm status $(helm last)`.
* [Helm Blob](https://github.com/C123R/helm-blob) ⭐ 8 | 🐛 0 | 🌐 Go | 📅 2022-02-09 - Plugin that allows you to manage helm repositories on the blob storage like Azure Blob, GCS, S3, etc.

## Tools, Extras

Helm-related tools

* [Helmfile](https://github.com/roboll/helmfile) ⭐ 4,035 | 🐛 527 | 🌐 Go | 📅 2023-04-27 - Helmfile is a declarative spec for deploying helm charts, supports flexible templating scenarios
* [Brigade](https://github.com/brigadecore/brigade) ⭐ 2,411 | 🐛 31 | 🌐 Go | 📅 2023-03-07 - A tool for running scriptable, automated tasks in the cloud — as part of your Kubernetes cluster
* [Helm Docs](https://github.com/norwoodj/helm-docs) ⭐ 1,757 | 🐛 97 | 🌐 Go | 📅 2026-06-22 - Auto-generates documentation from helm charts into markdown files
* [Helmify](https://github.com/arttor/helmify) ⭐ 1,743 | 🐛 56 | 🌐 Go | 📅 2026-05-07 - Generates a Helm chart from Kubernetes yamls
* [Helmsman](https://github.com/Praqma/helmsman) ⭐ 1,495 | 🐛 2 | 🌐 Go | 📅 2026-08-16 - Helmsman provides a declarative way of installing charts, features terraform-like desired state file approach and security enhancements
* [Monocular](https://github.com/helm/monocular) ⚠️ Archived - A web-based application that enables the search and discovery of charts from multiple Helm Chart repositories
* [Chart Releaser](https://github.com/helm/chart-releaser) ⭐ 784 | 🐛 66 | 🌐 Go | 📅 2026-07-27 - Helps Turn GitHub Repositories into Helm Chart Repositories
* [Ship](https://github.com/replicatedhq/ship) ⚠️ Archived - A tool that makes it easy to watch and apply updates to Helm charts and integrates [Kustomize](https://kustomize.io) patches and overlays
* [Reckoner](https://github.com/FairwindsOps/reckoner) ⭐ 354 | 🐛 12 | 🌐 Go | 📅 2026-08-16 - Reckoner is a tool to simplify management and installation of multiple Helm chart releases
* [Kubesafe](https://github.com/Telemaco019/kubesafe) ⭐ 333 | 🐛 0 | 🌐 Go | 📅 2026-08-09 - Safely manage multiple Kubernetes clusters by defining safe contexts and protected commands.
* [Readme Generator](https://github.com/bitnami-labs/readme-generator-for-helm) ⭐ 311 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-13 - Autogenerate Helm Charts READMEs' tables based on values YAML file metadata.
* [KubeStellar Console](https://github.com/kubestellar/console) ⭐ 128 | 🐛 28 | 🌐 TypeScript | 📅 2026-08-17 - Multi-cluster Kubernetes dashboard with Helm chart deployment, deployed via its own Helm chart for easy installation
* [Helm-Starter-Istio](https://github.com/salesforce/helm-starter-istio) ⭐ 92 | 🐛 3 | 🌐 Shell | 📅 2026-06-02 - A helm starter for creating [Istio](https://istio.io/) managed services
* [Helm Broker](https://github.com/kyma-project/helm-broker) ⚠️ Archived - A Service Broker which exposes Helm charts as Service Classes in the [Service Catalog](https://svc-cat.io/)
* [Chart Viewer](https://github.com/ecojuntak/chart-viewer) ⭐ 18 | 🐛 2 | 🌐 Go | 📅 2023-10-23 - Helps you inspect and compare chart template and also rendered manifest
* [Kube Foundry](https://github.com/kube-foundry/kube-foundry) ⭐ 17 | 🐛 3 | 🌐 Go | 📅 2026-04-01 - Kubernetes operator that runs AI coding agents (Claude Code, Codex, Cursor, Gemini, OpenCode) in sandboxed pods. Deploys via Helm chart.
* [segspec](https://github.com/dormstern/segspec) ⭐ 16 | 🐛 0 | 🌐 Go | 📅 2026-05-06 - Extracts network dependencies from Helm charts and other config files, generates Kubernetes NetworkPolicies with evidence tracing
* [Qovery](https://www.qovery.com/) - Enterprise Kubernetes management platform that natively deploys Helm charts from public/private repositories or Git repos. Includes Terraform provider, CLI, API, and [AI Agent Skill](https://github.com/Qovery/qovery-skills) ⭐ 9 | 🐛 4 | 🌐 Shell | 📅 2026-08-03 for AI-assisted deployment.
* [Keel.sh](https://keel.sh) - Continuous delivery for Kubernetes - enhances Helm with auto upgrades and other cool features
* [ChartMuseum](https://chartmuseum.com/) - ChartMuseum is an open-source, easy to deploy, Helm Chart Repository server.
* [werf](https://werf.io/) - A CLI tool for implementing CI/CD best practices using an extended version of Helm under the hood for deployment
* [YAML Validator](https://yamlvalidator.dev) - Online YAML validator and [Chrome extension](https://chromewebstore.google.com/detail/yaml-validator/gjgbohnlhijomhfiflapnlnmcpckgigg) with JSON Schema support for Helm Charts, Kubernetes, and other formats, plus YAML code folding on GitHub

## Testing

Testing Helm charts

* [`ct`, Official CLI for testing](https://github.com/helm/chart-testing) ⭐ 1,639 | 🐛 6 | 🌐 Go | 📅 2026-08-13 - CLI tool for linting and testing Helm charts.
* [helm-unittest](https://github.com/helm-unittest/helm-unittest) ⭐ 1,383 | 🐛 78 | 🌐 Go | 📅 2026-08-03 - BDD styled unit test framework for Kubernetes Helm charts as a Helm plugin.
* [helm-chartsnap](https://github.com/jlandowner/helm-chartsnap) ⭐ 111 | 🐛 16 | 🌐 Go | 📅 2026-08-03 - Snapshot testing tool for Helm charts. Allows you to compare the rendered output of a Helm chart against a snapshot.
* [Helm Test](https://helm.sh/docs/topics/chart_tests/) - Helm test command runs tests for a release. Mainly validates if the resources are created and available.
* [Helm Lint](https://helm.sh/docs/helm/helm_lint/) - Helm lint command checks a chart for possible issues.

## Community

Forums, discussion groups, SO tags.

* [Helm Slack](http://slack.k8s.io/) - #helm-users channel on Kubernetes Slack
* [StackOverflow Kubernetes-Helm](https://stackoverflow.com/questions/tagged/kubernetes-helm) - Stack Overflow threads tagged kubernetes-helm
* [StackOverflow Helm](https://stackoverflow.com/questions/tagged/helm) - Stack Overflow threads tagged Helm

# Contributing

Contributions are most welcome!

This list is just getting started, please contribute to make it super awesome.

Check out the [Contributing Guidelines](https://github.com/cdwv/awesome-helm/blob/master/CONTRIBUTING.md) ⭐ 1,111 | 🐛 8 | 📅 2026-05-16.

# License

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/InteractiveResource" property="dct:title" rel="dct:type">awesome-helm</span> by <a xmlns:cc="http://creativecommons.org" href="https://codewave.eu" property="cc:attributionName" rel="cc:attributionURL">CodeWave</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

# Maintainers

[<img width="300" title="Codewave.eu" src="cdwv-logo-new.svg">](https://codewave.eu)

Project is currently maintained, in our spare time, by [codewave.eu](https://codewave.eu) and a growing number of Contributors!

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-17._
