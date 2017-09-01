---
layout: page
title: Software Containers 
permalink: /containers/
---
# Overview
IDIA software on virtual machines is available and managed using [Singularity][singularity] containers. You can find
out more about what's available and how to use them on our dedicated [Github][github-containers]
repository.

### Available Containers
As of September 2017 the following containers are available:
* `casa-stable`
  * Access: Terminal (SSH).
  * The most recent, stable build of **CASA**, and can only be used on
  the terminal (e.g., by SSH'ing into the machine). Includes *MPI* support.
* `idia-jupyter-casa`
  * Access: Jupyter (https).
  * A working development version of CASA which is controlled through the Jupyter Notebook.  Open a new notebook with this kernel to
  run casa as a python module in a jupyter notebook.
* `idia-python-2.7`
  * Access: Terminal (SSH) and Jupyter (https).
  * Basic Python 2.7 stack.
* `idia-python-3.6`
  * Access: Terminal (SSH) and Jupyter (https).
  * Basic Python 3.6 stack.
* `kern2`
  * Access: Terminal (SSH) and Jupyter (https).
  * A comprehensive radio astronomy software environment that has **all** the packages in the
* `source-finding`
  * Access: Terminal (SSH) and Jupyter (https).
  * Includes commonly used tools for source-finding and data inspection including pyBDSF and AEGEAN. For more details consult
    our open [Github Issue][sfissues] on the topic.

### Running Containers

All base cloud image for IDIA will include singularity and also be added to the sudoers environment.  To run a container
from the command line simply enter `singularity run <container>`, for example to run the casa-stable container

* `singularity run casa-stable.img`

From the Jupter Hub simply open a notebook selecting the desired container from the `new` menu. 

### Reporting a bug / Requesting Software
Visit our [Github][github-containers] repo and open an **Issue**. 
#### Reporting a bug
Please provide a sensible report, which a relevant excerpt of an error message. Please provide
details on the expected behaviour, and possible ideas on how to fix the bug. 
#### Requesting Software
Provide the **name** of the package, the **location** or **link** to the repository or website, and
the name of the *existing* or *new* container in which to install the software package. 






[singularity]: http://singularity.lbl.gov/
[github-containers]:https://github.com/AfricanResearchCloud/idia-containers
[kern2]: http://kernsuite.info/
[sfissues]: https://github.com/AfricanResearchCloud/idia-containers/issues/4
