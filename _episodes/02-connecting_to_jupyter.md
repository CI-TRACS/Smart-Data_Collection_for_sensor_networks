---
title: "Connecting to Jupyter"
teaching: 5
exercises: 5
questions:
- "How do we deploy and access a Jupyter notebook server using MANA?"
objectives:
- "Use MANA's web interface to deploy a Jupyter notebook server job and connect to the server."
keypoints:
- "MANA's web interface provides a built in function for deploying a Jupyter notebook server."
- "After configuring and submitting a job to MANA for deploying the Jupyter notebook server, we can connect to the server and use it to access notebook files stored in the user's home directory."
---

# Creating a Jupyter notebook server

We will use MANA to deploy and access a Jupyter notebook with python scripts demonstrating the usage of the Tapis Streams API. The web interface for MANA includes a built in interface for creating and deploying a Jupyter notebook server.

## Deploying a Jupyter notebook server on MANA

Go to [https://uhhpc.its.hawaii.edu/](https://uhhpc.its.hawaii.edu/) in a web browser and log in with your UH credentials. This will bring you to the MANA web interface.

At the top of this interface there should be a dropdown menu labeled "Interactive Apps". Click this and select "Jupyter Notebook" from the dropdown menu. This will bring you to a form for configuring and deploying the server as a job on MANA.

![MANA Interactive job menu](/fig/mana_jupyter.PNG)

We will deploy this job to the sandbox? partition. Most of the default settings for this job should work, but increase the "Number of hours" to 2. These values should be as follows:

| Syntax                    | Description |
| ------------------------- | ----------- |
| SLURM Account             |             |
| Partition                 | sandbox?    |
| Number of hours           | 2           |
| Number of cores           | 4           |
| GB of RAM                 | 8           |
| Number of GPUs requested  | 0           |
| GPU Type                  | Any         |

Click the "Launch" button to schedule the job. This should display a tile with information about the job including its status. The job will likely start with the "Queued" status indicating that it has been queued and is waiting for resources to become available to execute the job.

![Jupyter notebook server job queued](/fig/job_queued.PNG)

Shortly, the job status should change to "Running" indicating the job has been launched, and a "Connect to Jupyter" button should be available at the bottom of the tile. Clicking this will connect you to the deployed Jupyter notebook server.

![Jupyter notebook server job running](/fig/job_running.PNG)

The Jupyter notebook server will display the files available in your account's home directory on MANA. We will need to download the notebook file for this workshop and install some dependencies the notebook relies on. The next sectin will describe how to install these dependencies and load the notebook.
