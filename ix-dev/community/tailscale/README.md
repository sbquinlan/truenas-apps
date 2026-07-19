# Tailscale

[Tailscale](https://tailscale.com) Secure remote access to shared resources

- When `Userspace` is **disabled**, `Tailscale` will run with `/dev/net/tun` device mounted from the host.
- Tailscale Services can optionally forward TCP ports to applications published on the NAS. Define each Service
  and its TCP ports in the Tailscale admin console first, authenticate this node with a tag-based identity, and
  approve the Service advertisement or configure an auto-approver policy.
