---
title: "Introduction"
teaching: 0
exercises: 0
questions:
- "Key question (FIXME)"
objectives:
- "First learning objective. (FIXME)"
keypoints:
- "First key point. Brief Answer to questions. (FIXME)"
---

# Streaming Data Collection for Sensor Networks



## Tapis

Tapis is a National Science Foundation (NSF) funded web-based API framework for securely managing computational workloads across infrastructures and institutions, so that experts can focus on their research instead of the technology needed to accomplish it. As part of work funded by the NSF starting in 2019, Tapis is delivering a version 3 (“V3”) of its platform with several new capabilities, including a multi-site security kernel, streaming data APIs, and high-level support for containerized applications.

Tapis provides FaaS through Abaco, which is based on the actor model of concurrent computation and Docker; users define computational primitives called \textit{actors} with a Docker image, and Abaco assigns each actor a unique URL over which it can receive messages. Users send the actor a message by making an HTTP POST request to the URL. In response to an actor receiving a message, Abaco launches a container from the associated image, injecting the message into the container. Typically, the container execution is asynchronous from the message request, though Abaco does provide an endpoint for sending a message to an actor and blocking until the execution completes, providing synchronous execution semantics. Abaco maintains a queue of messages for each actor, and is capable of launching containers in parallel for a given actor when the actor is registered as \textit{stateless}. The functions run with an authenticated context that allows them to make requests to other Tapis APIs to perform actions such as data transfer or job submission.

## Streams API

Tapis V3 introduces a Streams API for representing physical sensor networks and streaming and handling reported data. The API provides data-driven event support for real-time datacoming throught the API.

![Tapis Streams API flowchart](/fig/tapis-v3-streams-api.png)

Organization...
The API is structured into a hierarchy of 

PROVIDE TABLES WITH THE PROPERTIES FOR EACH OBJECT

### Projects

This is the broadest organizational structure available in the Streams API. 

### Sites

### Instruments

Instruments represent the physical instruments/sensors available at a given site.

### Variables

(registered to the instrument?)
Instruments will typically record properties of the environment they are placed in and report out these values. For example, a climatological sensor station may record levels of rainfall, air temperature, and relative humidity for its location. These would each be stored as a variable. The variable objects provide metadata for each of these measred properties.

### Measurements

The final structure in the Streams API is the actual measurments recorded by the instruments. Measurement objects provide a 

Measurements are registered 



## Abaco Containers

## Event Handling
