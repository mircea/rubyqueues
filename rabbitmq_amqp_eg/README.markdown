RabbitMQ with AMQP
==================

Summary
-------

A powerful, sophisticated and modern standards-based message broker and messaging protocol.

Websites: [RabbitMQ server](http://www.rabbitmq.com/) and [Ruby 'tmm1-amqp' client](http://github.com/tmm1/amqp/tree/master).

PROS: Many compatible clients and servers. Clusterable queue servers. Many subscription options. Multiple protocols (AMQP, STOMP, SMTP, etc).

CONS: The RabbitMQ server is fine, but the tmm1-amqp client uses an event-driven API that's tricky to work with and is somewhat inefficient (3X slower than Java AMQP client).

EVALUATION: A good choice for sophisticated message queuing.

Setup
-----

Install from: [http://www.rabbitmq.com/server.html](http://www.rabbitmq.com/server.html)

Sample code
-----------

* [Put and get a message](putget.rb)
* [Run naive benchmark](bench.rb)
