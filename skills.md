# Skills

A list of my skills broken down by category.

Some of these are tools/projects I've used (or use) and have enough experience with to deploy and manage in production, so enjoy my wonderful descriptions and Canadian humor.

## Programming Languages

In order of preference and experience.

- [Go](https://go.dev/)
  - My happy place, this is where a majority of my work gets done.
- [TypeScript](https://www.typescriptlang.org/) (inc. JavaScript)
  - I don't like JavaScript or TypeScript, but I tolerate them.
- [PHP](https://www.php.net/)
  - Not my preferred language, but I use it enough building [Pterodactyl](https://github.com/pterodactyl) to keep it in my arsenal.
- [Java](https://www.java.com/en/)
  - First language I learned and used professionally, not something I use much anymore.
- Shell
  - For when you need to quickly write some cursed automation that is "temporary" but never gets replaced by a proper solution.

## Frameworks

- [Laravel](https://laravel.com/)
  - Makes PHP more bearable, wouldn't write PHP without it.
- [React](https://react.dev/) (inc. [Remix](https://remix.run/))
  - I prefer Vue, but have worked a lot with React while building [Pterodactyl](https://github.com/pterodactyl) and a fair few number of other projects.
- [Vue.js](https://vuejs.org/) (inc. [Nuxt](https://nuxt.com/))
  - My preferred frontend framework of choice.

## Infrastructure

- [Ansible](https://www.ansible.com/)
  - Not something I personally use, but I have written and used multiple playbooks both personally and professionally in the past to manage large fleets of servers.
- Container Runtimes (Docker, Podman, or the CRI equivalents; containerd and CRI-O)
  - The thing that runs those juicy containers, or attempts to do so until you get blocked by AppArmor or SELinux.
  - I've built a fair number of apps that either mange containers or run inside of them, naturally I also have a lot of experience writing Container/Dockerfiles, though I do build most of my containers using [Nix](https://nixos.org/guides/how-nix-works).
- [Kubernetes](https://kubernetes.io/)
  - It's not perfect, but it's the best solution out there for managing massive amounts of containers.  I'm definitely the type of person to run a single website on a Kubernetes cluster, just because I can.
- [Terraform](https://www.terraform.io/)
  - [f**k HashiCorp and their license change](https://blog.gruntwork.io/the-future-of-terraform-must-be-open-ab0b9ba65bca), but other than that it's a great tool for provisioning all sorts of resources and infrastructure.

## Databases and Stores

- [MariaDB](https://mariadb.org/)
  - General-purpose SQL database, I use this when apps only support MySQL, otherwise I prefer using PostgreSQL instead.
- [PostgreSQL](https://www.postgresql.org/)
  - General-purpose SQL database, this is what I use for a majority of my applications that require an SQL database.
- [Redis](https://redis.io/)
  - That in-memory data store that eats memory.  I use this for caching or storing non-critical data that can always be recreated.
- [MeiliSearch](https://github.com/meilisearch/meilisearch)
  - I used MeiliSearch as the main data store for a blockchain indexer, it's fast and reliable but could use some sort of replication/horizontal scaling.

## Kubernetes

- [Helm](https://helm.sh/)
  - I don't like writing charts, but I do know how they work and how to deploy them.
- [FluxCD](https://fluxcd.io/) - GitOps for Kubernetes
  - This is what I use on all of my clusters to manage resources.

## Cloud Providers

- [AWS](https://aws.amazon.com/)
  - My preferred big cloud provider, though I do prefer just running my own metal.
- [Cloudflare Workers](https://workers.cloudflare.com/)
  - I have built quite a few apps that run on Cloudflare Workers, it's great for anything that can run on the edge and isn't latency sensitive.

## Linux Distributions

I am fully capable of SSHing into a server and managing it.  I daily-drive NixOS and deal with Linux servers on a daily basis.

- [NixOS](https://nixos.org/)
  - NixOS is my preferred desktop and server distribution, and it's what I daily-drive.  It's designed around reproducibility and is wonderful for managing servers.
- [Red Hat Enterprise Linux](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux)
  - General workhorse for when I want something to just work.  This is what I primarily use when NixOS is not an acceptable choice.
- [Debian](https://www.debian.org/)
  - Another good option, I prefer RHEL but have worked quite a lot with Debian as well.

## Tools

- [Git](https://git-scm.com/)
  - `git push --force --set-upstream origin master`
- [Nix](https://nixos.org/guides/how-nix-works)
  - I love Nix, it makes building and developing software so much easier.  If you like consistent package versions and reproducible builds, this one is for you.  Almost all of my projects have Nix setup for development environments and even some for building release artifacts.  You can even use it to build distroless container images.
- [Tailwind CSS](https://tailwindcss.com/)
  - Some people hate it, but I love it.  It's my preferred way of styling frontends, it's essentially legible inline-CSS.

## Protocols

- [Connect](https://connectrpc.com/)
  - Uses Protobuf (or JSON) over HTTP (HTTP/2 not required), works in the browser.
- [gRPC](https://grpc.io/)
  - If you are using this, you have reached peak complexity.
- HTTP
  - 419 I'm a Teapot

## Observability

- [Grafana](https://grafana.com/)
  - For all those sexy dashboards you stare at when prod is down.  Assuming your monitoring stack is still online.
  - [Loki](https://grafana.com/oss/loki/)
    - For figuring out why your app is throwing 500 errors, assuming you added proper logging in the first place.
  - [Mimir](https://grafana.com/oss/mimir/)
    - Prometheus, but built to store a metric f**kton of timeseries.  See what I did there? :)
  - [Tempo](https://grafana.com/oss/tempo/)
    - Traces for knowing why your application's response time is 5 minutes long.
- [Prometheus](https://prometheus.io/)
  - If you aren't sampling at `1s` you're missing out on large amounts of CPU, Memory, and Storage usage.

## Continuous Integration (CI)

- [GitHub Actions](https://github.com/features/actions)
  - What I use for all of my CI pipelines.

## Networking

I'm still convinced that networking is black-magic, powered by blood sacrifice and fear.

- BGP
  - I have a bit of experience with using BGP, and enough knowledge to know that if it's not DNS, it's BGP.
- DNS
  - It's not dns
  - There's no way it's DNS
  - It was DNS
- SMTP
  - Don't ask my why I know this, but in the past I thought it would be fun to build a mail server from scratch and I spent way too much time reading and implementing SMTP (and the extensions) RFCs using Go.  Then in typical programmer fashion, I never fully finished or open-sourced it and moved onto other projects instead.

## Storage

Storage terrifies me, you neglect it until it becomes a problem, then you never want to worry about it or touch it again.

- [Ceph](https://ceph.com/en/)
  - My goto storage solution for when you need reliable and distributed storage.
