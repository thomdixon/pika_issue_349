# pika_issue_349
Code to reproduce issue #349 in pika/pika

# Conclusion
Turns out that issue [#349](https://github.com/pika/pika/issues/349) was a duplicate of [#507](https://github.com/pika/pika/issues/507), which was addressed in pull request [#509](https://github.com/pika/pika/pull/509) and is fixed in the current master, but not the 0.9.14 release.

Also of interest, [@vitaly-krugl](https://github.com/vitaly-krugl) noticed that this script can possibly hard-crash RabbitMQ 3.2:

>Hi @thomdixon, your test turned out to be a great way to hard-crash RabbitMQ 3.2.0 when running with the tip-of-master pika that doesn't have those framing issues. It crashed RabbitMQ reliably after about 30 minutes. The good news is that RabbitMQ 3.5.0 didn't crash under that type of load. FYI
