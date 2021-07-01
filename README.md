# kubernetes-the-not-so-hard-way

Kubernetes - The not so hard way

Welcome to a short guide to set up a "bare metal" stand-alone Kubernetes cluster

If you want to sandbox your own Kubernetes cluster, let's go.

What we need, 2 workstations/servers :
  + 1 PlaneControl
   + OS : Debian
   + CPU Cores : 2
   + Minimal RAM : 2 Go
   ++ Optionally, without Swap (we will disable it if there's one)
  + 1 Pod
   + Same as PlaneControl, but
   + Minimal RAM : 4 Go
   ++ Optionnaly, without Swap

[Initial setup before Kuberneting](01_InitialSteps_All.md)
[Kubernetes initialisation: Init PlaneControl](02_Kubernetes_Init.md)
[Kubernetes initialisation: Add a Pod](03_Kubernetes_Pod_Join.md)
[Kubernetes Dashboard](04_Kubernetes_Dashboard.md)
[Kubernetes CLI Completion](05_Kubernetes_CLI_Completion.md)

