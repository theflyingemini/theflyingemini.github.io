---
layout:     post   				             # 使用的布局（不需要改）
title:      What is a Message Queue    # 标题
subtitle:                              # 副标题
date:       2021-06-01 				         # 时间
author:     Roger 						         # 作者
header-img: img/post-bg-o.jpeg         # 这篇文章标题背景图片
catalog:    true 						           # 是否归档
tags:								                   # 标签
    - Distributed System
---

#

[What is a Message Queue?](https://aws.amazon.com/message-queue/)

A message queue is a form of asynchronous service-to-service communication used in serverless and microservices architectures. Messages are stored on the queue until they are processed and deleted. Each message is processed only once, by a single consumer. Message queues can be used to decouple heavyweight processing, to buffer or batch work, and to smooth spiky workloads.

Message queues can significantly simplify coding of decoupled applications, while improving performance, reliability and scalability.

Message queues allow different parts of a system to communicate and process operations asynchronously.

A message queue provides a lightweight buffer which temporarily stores messages, and endpoints that allow software components to connect to the queue in order to send and receive messages.

The messages are usually small, and can be things like requests, replies, error messages, or just plain information.

To send a message, a component called a producer adds a message to the queue. The message is stored on the queue until another component called a consumer retrieves the message and does something with it.

Many producers and consumers can use the queue, but each message is processed only once, by a single consumer. For this reason, this messaging pattern is often called one-to-one, or point-to-point, communications.

When a message needs to be processed by more than one consumer, message queues can be combined with Pub/Sub messaging in a fanout design pattern.

See “ [What is Pub/Sub messaging?](https://aws.amazon.com/pub-sub-messaging/) “ for details, and visit our  [Amazon Simple Notification Service (SNS)](https://aws.amazon.com/migration-acceleration-program/)  website for an overview of Pub/Sub messaging on AWS.
