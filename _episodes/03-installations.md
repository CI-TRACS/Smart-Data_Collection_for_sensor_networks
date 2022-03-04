---
title: "Installations"
teaching: 5
exercises: 5
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
![Jupyter Home, "New" button selected](../fig/jupyter_home_new_outlined.png) 

Next, click "Terminal" from the drop-down bar.
![Jupyter Home, "Terminal" button selected](../fig/jupyter_home_new_terminal_outlined.png)

You should now be brought to a terminal connected to the virtual machine.

> ### Heads-up!
> On your first time using a MANA terminal, it will show a "do you trust this system" prompt, simply type "yes" and enter.
{: .callout}

![Jupyter Terminal](../fig/jupyter_terminal_start.png)
Now that we have a terminal, it's time to install some python packages!

---

Let's install the `tapipy` package, which includes functions that help us work with the Tapis system.
Run the following command:
```bash
python -m pip install tapipy
```

> #### What this does...
> This runs python and tells it to execute the "pip" module, then tells pip to install tapipy.

![Install Tapipy](../fig/jupyter_terminal_install_tapipy.png)

When it's done, you should see the following:
![Installed Tapipy](../fig/jupyter_terminal_installed_tapipy.png)

# Getting the Notebook

We're going to use `git` to download the latest version of the Jupyter Notebook for this workshop.
Git is an application that helps with collaborative software development.
Its `clone` command allows us to download the entire project folder (called a Repository) in a simple and reproducible manner.

Run the following command:
```bash
git clone https://github.com/CI-TRACS/Smart-Data_Collection_for_sensor_networks_notebook.git
```

![Clone the Tapis Jupyter Repository](../fig/jupyter_terminal_clone_notebook.png)

It will take a few seconds to load, then you should see the following.

![Cloned the Tapis Jupyter Repository](../fig/jupyter_terminal_cloned_notebook.png)

Now, let's get to editing the notebook! 

---

# Editing the Notebook
Now that we've cloned the notebook repository to the `~/Smart-Data_collection_for_sensor_networks_notebook` directory, it's time to go there and open up the notebook.


Go back to the Jupyter Home interface, where you should see a screen like this:
![Jupyter Home Interface With notebook repo](../fig/jupyter_home_with_notebook.png)

Click `Smart-Data_Collection_for_sensor_networks_notebook` to enter our newly downloaded folder.



The new folder includes our notebook, and any other files we will happen to need.
![Jupyter File Manager in repo](../fig/jupyter_file_manager_in_notebook_repo.png)

Finally, click the `Smart-Data_Collection_for_sensor_networks.ipynb` file to open our notebook.


The notebook should now be open, and ready to edit!
![Tapis Streams Jupyter Notebook Opened](../fig/notebook_open.png)

{% include links.md %}
