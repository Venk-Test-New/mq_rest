The Message
======================================

The primary goal of the CourierREST protocol is to produce and to consume messages. Therefore the Courier message plays a central role of the CourierREST protocol.

Courier messages are not very different from other messaging protocols messages. A CourierREST message has three parts: headers, properties, and a payload.

    ┌────────────────┐
    │    Headers     │
    ├────────────────┤
    │   Properties   │
    ├────────────────┤
    │                │
    │                │
    │    Payload     │
    │                │
    │                │
    └────────────────┘

A Courier message has three elements: a header, properties, and a body. The mandatory parts are the properties and the body.

* Headers, courier defined metadata
* Properties, user defined metadata
* Body, payload of the message


Headers
--------------------------------------

Courier message properties can be used to add custom information that does not belong, although it is probably related, to the payload.



Properties
--------------------------------------

Courier-specific properties like `lockId`, `messageId`, or `deliveryCount`.


Payload
--------------------------------------

Courier messages can only carry one kind of payload, a stream of uninterpreted bytes. This enables with proper encoding to send and to receive data in many different forms.
