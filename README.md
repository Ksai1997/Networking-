# Networking in DevOps — Field Notes

A responsive, slide-style training website for an internal engineering session. It covers networking foundations, containers, Kubernetes networking and policy, observability, and a troubleshooting exercise. The page is plain HTML, CSS, and JavaScript; it needs no build step or runtime dependencies.

## Run locally

Open `index.html` in a browser, or serve the folder with any static file server. Keyboard navigation uses the left/right arrows; the course map button shows every slide.

## Course outline

The interactive guide now has 23 slides (about 65 minutes): OSI layers, TCP/IP mapping and encapsulation, IPv4/IPv6 and CIDR, routing/ARP/NAT, DNS recursion, TCP handshakes/flow and congestion control, HTTP/TLS, a browser-to-Pod request walkthrough, firewalls/VPNs, load balancers/proxies/CDNs, TCP/UDP, Docker, Kubernetes Services and policies, observability, a practical troubleshooting exercise, and an in-site reader for all 11 original A-to-Z chapters.

## Publish with GitHub Pages

This repository includes a GitHub Actions workflow for publishing the site as a static GitHub Pages site.

1. Create a **public** GitHub repository and push these files to its `main` branch.
2. In the repository, open **Settings → Pages** and choose **GitHub Actions** as the build and deployment source.
3. The workflow publishes on pushes to `main`. Open **Actions** to see when the first deployment finishes; the Pages URL appears in the deployment summary.

GitHub Pages offers free static hosting for public repositories. If your training content or audience must remain private, host it behind your organization’s access controls instead. This site contains no internal company material as written.

## Content sources

- [A to Z of Networking for DevOps](https://github.com/iam-veeramalla/a-to-z-of-networking/tree/main) — the requested open source learning path. The Source Chapters slide loads the original Markdown lesson text from the repository and renders it inside the training site, preserving its wording, examples, commands, and attribution. Internet access is required to load those chapters. The repository is MIT licensed.
- [Kubernetes Services, Load Balancing, and Networking](https://kubernetes.io/docs/concepts/services-networking/)
- [Kubernetes Cluster Networking](https://kubernetes.io/docs/concepts/cluster-administration/networking/)
- [Container Network Interface](https://github.com/containernetworking/cni)
- [Cilium](https://github.com/cilium/cilium)
- [Computer Networking: Principles, Protocols and Practice](https://github.com/SystemsApproach/book)
- Video channels: [Kubernetes](https://www.youtube.com/@KubernetesCommunity), [CNCF](https://www.youtube.com/@CNCF), [TechWorld with Nana](https://www.youtube.com/@TechWorldwithNana), [Practical Networking](https://www.youtube.com/@PracticalNetworking)

## License

MIT. See [LICENSE](LICENSE).
