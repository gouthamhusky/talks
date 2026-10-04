# Grafana for Kubernetes-based platforms: every cluster, every region, one dashboard

**[Grafana & Friends Austin — Autumn of Observability](https://www.meetup.com/grafana-friends-austin-meetup-group/events/316372961/)**
· September 22, 2026 · Austin, TX

- Slides: [PowerPoint](grafana-for-kubernetes-platforms.pptx)
- [LinkedIn post](https://www.linkedin.com/posts/goutham-kanags_i-just-finished-presenting-my-talk-on-grafana-ugcPost-7508382117324623873-Vtz4/)
- [Talk page](https://gouthamhusky.github.io/blogsite/talks/grafana-for-kubernetes-platforms/)

A tenant cluster is stuck: which one, in which region, and why? On a
platform built from operators, the answer is already written down. Every
reconcile loop writes status conditions back onto the resource. This talk
exports those conditions as Prometheus time series (one gauge, the condition
as a label, `min` to aggregate) and builds one Grafana dashboard for the
whole fleet, across every cluster and every region.
