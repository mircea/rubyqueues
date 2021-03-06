Ruby message queue showdown
===========================

Updated: 2009-04-17

Summary
-------

Using message queues effectively can significantly improve the efficiency and responsiveness of applications. Ruby programmers are lucky to have many messaging options to choose from, but are cursed with having to pick between them. These documents and source code samples attempt to provide basic information to help Ruby programmers better understand these alternatives.

Details
-------

* [Comparison table of message queues](http://wiki.github.com/igal/rubyqueues)
* [ActiveMQ with Stomp](./master/activemq_stomp_eg/)
* [Beanstalkd](./master/beanstalkd_eg/)
* [Delayed::Job](./master/delayed_job_eg/)
* [Kestrel](./master/kestrel_eg/)
* [MemcacheQ](./master/memcacheq_eg/)
* [RabbitMQ with AMQP](./master/rabbitmq_ampq_eg/)
* [Sparrow](./master/sparrow_eg/)
* [Starling](./master/starling_eg/)

Caveat emptor
-------------

I have not used most of these messaging systems outside this evaluation, so please perform your own analysis before making an important decision. I'll gladly incorporate additional information and corrections that you send me so that I can accurately represent each alternative.

The naive benchmark does NOT acurately represent the performance of these systems under a realistic workload. This naive benchmark simply has a single client making sequential calls, whereas a realistic workload would include a large number of clients working in bursts. For example, Starling is much faster than Kestrel when talking to a few clients, while Kestrel is allegedly much faster than Starling when talking to a large number of clients.
