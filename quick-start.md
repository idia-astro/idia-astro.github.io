---
layout: page
title: Quick Start 
permalink: /quick-start/
---

The VM for your project will be assigned a name **projectVM** and can accessed as the **projectVM**.idia.ac.za.

## Jupyter-Hub
* Go to [https://projectVM.idia.ac.za][helo] in your preferred browser. 
* Login with your LDAP username/password.
* Simply choose the container that you want to use from your Jupyter Hub dashboard. A Jupyter
  Notebook corresponding to the container will open up.

## Terminal

* SSH as follows: `ssh -Y -i /path/to/your/key projectvm.idia.ac.za -l <your-username>`.
* The containers can be found in the following path: `/data/exp_soft/containers/`
* To jump into a container shell, you can use the command: `singularity shell
  /path/to/container.img`.

[helo]: https://helo.idia.ac.za
