# kubernetes-the-not-so-hard-way

Kubernetes - The not so hard way

Welcome to a short guide to set up a "bare metal" stand-alone Kubernetes cluster

If you want to sandbox your own Kubernetes cluster, let's go.

What we need, 2 workstations/servers :
  - 1 PlaneControl
   - OS : Debian
   - CPU Cores : 2
   - Minimal RAM : 2 Go
   -- Optionally, without Swap (we will disable it if there's one)
  - 1 Pod
   - Same as PlaneControl, but
   - Minimal RAM : 4 Go
   -- Optionnaly, without Swap

01 InitialSteps_All
02 Kubernetes_Init
03 Kubernetes_Pod_Join
04 Kubernetes_Dashboard
05 Kubernetes_CLI_Completion

