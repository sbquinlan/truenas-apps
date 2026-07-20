# Tailscale

[Tailscale](https://tailscale.com) Secure remote access to shared resources

- When `Userspace` is **disabled**, `Tailscale` will run with `/dev/net/tun` device mounted from the host.
- Tailscale Services can optionally expose applications published on the NAS. HTTPS endpoints terminate
  Tailscale-managed TLS and proxy to the application's backend port, so a Service on port 443 can reach an app
  published on a different port. Define each Service and its ports in the Tailscale admin console first, enable
  HTTPS for the tailnet when using HTTPS endpoints, authenticate this node with a tag-based identity, and approve
  the Service advertisement or configure an auto-approver policy.
