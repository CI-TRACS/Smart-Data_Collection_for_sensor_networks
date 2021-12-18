---
title: "Installations"
teaching: 3
exercises: 3
questions:
- "How do we bring code libraries into our Jupyter notebook?"
objectives:
- "Open the HPC terminal in the browser."
- "Use `pip` to install python libraries."
- "Import libraries and test them out in a Jupyter notebook."
keypoints:
- "MANA's web interface provides a terminal for the machine that the notebook runs on."
- "You can install and import new python libraries to support a notebook."
---

# Installing Dependencies

To install python dependencies, we're going to use the `pip` utility.

First we'll want to open a terminal on the node that our notebook is running on.
To do this, go to the tab where you opened the notebook from, and click "New".
![Jupyter Home, "New" button selected](/fig/jupyter_home_new_outlined.png) 

Next, click "Terminal" from the drop-down bar.
![Jupyter Home, "Terminal" button selected](/fig/jupyter_home_new_terminal_outlined.png)

You should now be brought to a terminal connected to the virtual machine.

> ### Heads-up!
> On your first time using a MANA terminal, it will show a "do you trust this system" prompt, simply type "yes" and enter.
{: .callout}

![Jupyter Terminal](/fig/jupyter_terminal_start.png)
Now that we have a terminal, it's time to install some python packages!

---

Let's install the `tapipy` package, which includes functions that help us work with the Tapis system.
Run the following command:
```bash
python -m pip install tapipy
```

> #### What this does...
> This runs python and tells it to execute the "pip" module, then tells pip to install tapipy.
{: .solution}

![Install Tapipy](/fig/jupyter_terminal_install_tapipy.png)

When it's done, you should see the following:
![Installed Tapipy](/fig/jupyter_terminal_installed_tapipy.png)


{% include links.md %}

