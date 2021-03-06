# Rebar-friendly fork of Rabbit common

This is a fork of the rabbit_common dependency, which is needed by the
[official RabbitMQ/AMQP Erlang client](https://github.com/rabbitmq/rabbitmq-erlang-client).

It's meant to be included in your rebar projects in your rebar.config file:

    {deps, [
      {rabbit_common, ".*", {git, "git://github.com/jbrisbin/rabbit_common.git", "rabbitmq-3.5.6"}}
    ]}.

The "master" branch of this port is a simple re-packaging of the rabbit_common AMQP client dependency.

### License

This package, just like the the RabbitMQ server, is licensed under the MPL. For the MPL, please see LICENSE-MPL-RabbitMQ.

### Note

This is a dependency of amqp-client which is a dependency of ex-autorenewals.
Both amqp-client and rabbit-common are required to work around a compilation error that was introduced in Erlang 19.
See amqp-client repo for further information.
