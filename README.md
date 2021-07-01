# kubernetes-the-not-so-hard-way

Kubernetes - The not so hard way

Welcome to a short guide to set up a "bare metal" (:metal:) stand-alone Kubernetes cluster !

If you want to sandbox your own Kubernetes cluster, without any AWS, GCP or Azure account, let's go.

What we need, 2 servers :
 * 1 PlaneControl
   * OS : Debian
   * CPU Cores : 2
   * Minimal RAM : 2 Go
     * Optionally, without Swap (we will disable it if there's one)
 * 1 Pod
   * Same as PlaneControl, but
   * Minimal RAM : 4 Go
     * Optionnaly, without Swap

Kubernetes picked(/opinionated) options :
 * Container : Containerd (yes, not Docker)
 * Network Add-on : Weaver

:footprints: [First, let's disable the Swap](00_InitialSteps_All_DisableSwap.md)

:footprints: [Initial setup before Kuberneting](01_InitialSteps_All_Install.md)

:footprints: [Kubernetes initialisation: Init PlaneControl](02_Kubernetes_Init.md)

:footprints: [Kubernetes initialisation: Add a Pod](03_Kubernetes_Pod_Join.md)

:footprints: [Kubernetes Dashboard](04_Kubernetes_Dashboard.md)

:footprints: [Kubernetes CLI Completion](05_Kubernetes_CLI_Completion.md)

