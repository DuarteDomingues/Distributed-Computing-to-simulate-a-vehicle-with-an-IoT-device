# Distributed-Computing-to-simulate-a-vehicle-with-an-IoT-device
Distributed Systems project that works as a simulator of a vehicle with an IoT device, sending instantaneous speed messages to a system of event-based communication and group communication.

The system is divided in three layers:

* Generate events randomly with an unique identifier, a location, an event acquisition date, and the velocity value and speed at the given instant of time.
* Perform event-driven communication. To perform this communication RabbitMQ is used, in which there is a broker to 
where the messages are sent and each message is associated with an Exchange.
* Two groups of processes that work through group communication, where in this case the Spread middleware will be used. Spread 
performs group communication for distributed applications with reliable multicast and full causal ordering of messages, even in the presence of failures.
