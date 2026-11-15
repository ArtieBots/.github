# Security Policy

This policy covers every repository in the [ArtieBots](https://github.com/ArtieBots)
organization that does not have a security policy of its own.

## Supported versions

Artie is a research project under active development. Only the latest code on each
repository's `main` branch, and the latest published release of each package, receive
security fixes.

## Reporting a vulnerability

Please **do not** open a public issue for a security problem.

Report it privately instead, through GitHub: open the repository the problem is in, go to
its **Security** tab, and choose **Report a vulnerability**. Only the maintainers can see
the report.

Include what you can of:

- which repository and component is affected, and which version or commit
- what an attacker could do, and how
- steps to reproduce it, or a proof of concept

You should hear back within two weeks. Artie is maintained by volunteers, so a fix may take
longer than that, but you will be kept informed, and credited in the fix unless you would
rather not be.

## Scope

Artie runs on a robot's own Kubernetes cluster, usually on a private network. Reports are
most useful when they concern something an Artie deployment exposes - the API server, the
services and drivers on the cluster, the daemons on the admin and compute nodes, or the
controller node's Yocto image - or the tools that build and deploy it (Artie Tool, Artie
Workbench, Artie CLI).
