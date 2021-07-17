# Resolving-Message-Logic-Dependencies-in-ROS
## Undergraduate Thesis
### Abstract
Robotic systems are event-based systems focusing at achieving high degrees of
autonomy. The final action taken is achieved through an accumulation of series of
computations by independent components in the system which can communicate with
each other by exchanging messages through channels.

State-of-the-art robotics frameworks provide a high-level architecture for message
communication so that the actual mechanism is hidden from the end user. This is
implemented through a system of publishers (message sources) and subscribers
(message sinks) for communication.

Since each node has the ability to subscribe or publish to any channel, there is no
direct lookup to see which components of a system are affected by changes in message
definition or message logic. By exploring previous work and introducing an efficient
method of program analysis, we worked towards a tool which can accurately resolve
such message logic dependencies in popular frameworks for robot software
development.

The communication between nodes relies on the messages being exchanged between
them, forming a network of publishers and subscribers. The performance of the
network can be defined in terms of latency and/or message drops. We investigate how
the message size affects the performance of the network.

For any given field in a message, it may or may not be utilised by a node. If it is not
used by any node in the system, we could prune that field and expect to see a rise in
performance of the network. We performed tests and worked towards a tool which
automatically detects unused fields and prunes them.

We also explored several other potential issues which could affect pace of
development, or cause unexpected crashes in the system.

- Please refer [Poster](./Poster.pdf) for short summary of the project.
- Refer [Report](./Report.pdf) for further details about the project.
