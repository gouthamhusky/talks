# Grafana for Kubernetes-based platforms: every cluster, every region, one dashboard

**[Grafana & Friends Austin — Autumn of Observability](https://www.meetup.com/grafana-friends-austin-meetup-group/events/316372961/)**
· September 22, 2026 · Austin, TX

- Slides: [PDF](grafana-for-kubernetes-platforms.pdf) · [PowerPoint](grafana-for-kubernetes-platforms.pptx)
- [LinkedIn post](https://www.linkedin.com/posts/goutham-kanags_i-just-finished-presenting-my-talk-on-grafana-ugcPost-7508382117324623873-Vtz4/)
- [Talk page](https://gouthamhusky.github.io/blogsite/talks/grafana-for-kubernetes-platforms/)

A platform team doesn't run one Kubernetes cluster. It runs its customers'
clusters: a fleet of them, spread across regions, each one provisioned and
reconciled by an operator on a management cluster. When a customer's cluster
gets stuck, the questions come fast. Which cluster? Which region? Stuck at
which stage? And whose is it?

The operator already knows. Every reconcile writes status conditions
(`InfrastructureReady`, `ArgoAppReady`, `Synced`) back onto the cluster
resource. This talk exports those conditions as Prometheus metrics (one
gauge, the condition as a label, `min` to aggregate) and turns them into a
single Grafana dashboard that answers those questions for every customer
cluster, in every region.
