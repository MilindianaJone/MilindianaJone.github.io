# GPU Learnings

Here's the table of contents:

1. TOC
{:toc}

## Devcontainer Setup

Setting up devcontainers on the local machines at UQ was a challenge but worked great once done. I followed Professor Brian Lovell's [guide](https://lovellbrian.github.io/2023/10/02/BYODImage.html) to get through the process. I did run into some issues, especially with using RDP. Sometimes I would setup most of the devcontainers over RDP on one desktop, get disconnected and have to redo everything on another desktop. 

I encountered an issue with one of the commands, asking me to input this:
```console
git clone --cpufrozen https://github.com/lovellbrian/course22
```

I identified the mistake and correctly inputted this command to get the cpufrozen branch.
```console
git clone --branch cpufrozen https://github.com/lovellbrian/course22
```

## Running GPUs

Using a CPU for my daily activities, it was great fun using the **Nvidia GeForce RTX 2080** powered GPUs available in the labs in 78-336. I experimented with different batch sizes:

 - 16
 - 32
 - 64
 - 128
 - 256

The GPU increased the training speed by more than 5 times for the maximum speedup as compared to the CPU.

| CPU | GPU |
|-|-|
| 16s | 3s |

# GPU Runtime Graphs

It was interesting to see the raw runtime usage of the GPUs through the `nvtop` command on linux.

![](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.linuxlinks.com%2Fnvtop-htop-task-monitor-amd-intel-nvidia-gpus%2F&psig=AOvVaw2V0ZwOTMrEq53NKC15n3UM&ust=1714157954880000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCOC-lpKG3oUDFQAAAAAdAAAAABAE)

## Footnotes

[^1]: This is the footnote.
