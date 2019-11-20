<p align="center">
  <img src="/gopher.png" height="400">
  <h1 align="center">
    Go Patterns
    <br>
    <a href="http://travis-ci.org/tmrts/go-patterns"><img alt="build-status" src="https://img.shields.io/badge/build-passing-brightgreen.svg?style=flat-square" /></a>
    <a href="https://github.com/sindresorhus/awesome" ><img alt="awesome" src="https://img.shields.io/badge/awesome-%E2%9C%93-ff69b4.svg?style=flat-square" /></a>
    <a href="https://github.com/tmrts/go-patterns/blob/master/LICENSE" ><img alt="license" src="https://img.shields.io/badge/license-Apache%20License%202.0-E91E63.svg?style=flat-square" /></a>
  </h1>
</p>

A curated collection of idiomatic design & application patterns for Go language.

## Creational Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Abstract Factory抽象工厂](/creational/abstract_factory.md) | Provides an interface for creating families of releated objects | ✘ |
| [Builder 生成器](/creational/builder.md) | Builds a complex object using simple objects | ✔ |
| [Factory Method 工厂模式](/creational/factory.md) | Defers instantiation of an object to a specialized function for creating instances | ✔ |
| [Object Pool 对象池模式](/creational/object-pool.md) | Instantiates and maintains a group of objects instances of the same type | ✔ |
| [Singleton 单例模式](/creational/singleton.md) | Restricts instantiation of a type to one object | ✔ |

## Structural Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Bridge桥接模式](/structural/bridge.md) | Decouples an interface from its implementation so that the two can vary independently | ✘ |
| [Composite 组合模式](/structural/composite.md) | Encapsulates and provides access to a number of different objects | ✘ |
| [Decorator 装饰器模式](/structural/decorator.md) | Adds behavior to an object, statically or dynamically | ✔ |
| [Facade 门面模式](/structural/facade.md) | Uses one type as an API to a number of others | ✘ |
| [Flyweight 享元模式](/structural/flyweight.md) | Reuses existing instances of objects with similar/identical state to minimize resource usage | ✘ |
| [Proxy 代理模式](/structural/proxy.md) | Provides a surrogate for an object to control it's actions | ✔ |

## Behavioral Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Chain of Responsibility 责任链模式](/behavioral/chain_of_responsibility.md) | Avoids coupling a sender to receiver by giving more than object a chance to handle the request | ✘ |
| [Command 命令模式](/behavioral/command.md) | Bundles a command and arguments to call later | ✘ |
| [Mediator 终结者模式](/behavioral/mediator.md) | Connects objects and acts as a proxy | ✘ |
| [Memento 备忘录模式](/behavioral/memento.md) | Generate an opaque token that can be used to go back to a previous state | ✘ |
| [Observer 观察者模式](/behavioral/observer.md) | Provide a callback for notification of events/changes to data | ✔ |
| [Registry 注册模式](/behavioral/registry.md) | Keep track of all subclasses of a given class | ✘ |
| [State 状态模式](/behavioral/state.md) | Encapsulates varying behavior for the same object based on its internal state | ✘ |
| [Strategy 策略模式](/behavioral/strategy.md) | Enables an algorithm's behavior to be selected at runtime | ✔ |
| [Template 模版模式](/behavioral/template.md) | Defines a skeleton class which defers some methods to subclasses | ✘ |
| [Visitor 访问者模式 ](/behavioral/visitor.md) | Separates an algorithm from an object on which it operates | ✘ |

## Synchronization Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Condition Variable](/synchronization/condition_variable.md) | Provides a mechanism for threads to temporarily give up access in order to wait for some condition | ✘ |
| [Lock/Mutex](/synchronization/mutex.md) | Enforces mutual exclusion limit on a resource to gain exclusive access | ✘ |
| [Monitor](/synchronization/monitor.md) | Combination of mutex and condition variable patterns | ✘ |
| [Read-Write Lock](/synchronization/read_write_lock.md) | Allows parallel read access, but only exclusive access on write operations to a resource | ✘ |
| [Semaphore](/synchronization/semaphore.md) | Allows controlling access to a common resource | ✔ |

## Concurrency Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [N-Barrier](/concurrency/barrier.md) | Prevents a process from proceeding until all N processes reach to the barrier | ✘ |
| [Bounded Parallelism](/concurrency/bounded_parallelism.md) | Completes large number of independent tasks with resource limits | ✔ |
| [Broadcast](/concurrency/broadcast.md) | Transfers a message to all recipients simultaneously | ✘ |
| [Coroutines](/concurrency/coroutine.md) | Subroutines that allow suspending and resuming execution at certain locations | ✘ |
| [Generators](/concurrency/generator.md) | Yields a sequence of values one at a time | ✔ |
| [Reactor](/concurrency/reactor.md) | Demultiplexes service requests delivered concurrently to a service handler and dispatches them syncronously to the associated request handlers | ✘ |
| [Parallelism](/concurrency/parallelism.md) | Completes large number of independent tasks | ✔ |
| [Producer Consumer](/concurrency/producer_consumer.md) | Separates tasks from task executions | ✘ |

## Messaging Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Fan-In](/messaging/fan_in.md) | Funnels tasks to a work sink (e.g. server) | ✔ |
| [Fan-Out](/messaging/fan_out.md) | Distributes tasks among workers (e.g. producer) | ✔ |
| [Futures & Promises](/messaging/futures_promises.md) | Acts as a place-holder of a result that is initially unknown for synchronization purposes | ✘ |
| [Publish/Subscribe](/messaging/publish_subscribe.md) | Passes information to a collection of recipients who subscribed to a topic | ✔ |
| [Push & Pull](/messaging/push_pull.md) | Distributes messages to multiple workers, arranged in a pipeline | ✘ |

## Stability Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Bulkheads](/stability/bulkhead.md)  | Enforces a principle of failure containment (i.e. prevents cascading failures) | ✘ |
| [Circuit-Breaker](/stability/circuit-breaker.md) | Stops the flow of the requests when requests are likely to fail | ✔ |
| [Deadline](/stability/deadline.md) | Allows clients to stop waiting for a response once the probability of response becomes low (e.g. after waiting 10 seconds for a page refresh) | ✘ |
| [Fail-Fast](/stability/fail_fast.md) | Checks the availability of required resources at the start of a request and fails if the requirements are not satisfied | ✘ |
| [Handshaking](/stability/handshaking.md) | Asks a component if it can take any more load, if it can't, the request is declined | ✘ |
| [Steady-State](/stability/steady_state.md) | For every service that accumulates a resource, some other service must recycle that resource | ✘ |

## Profiling Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Timing Functions](/profiling/timing.md) | Wraps a function and logs the execution | ✔ |

## Idioms

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Functional Options](/idiom/functional-options.md) | Allows creating clean APIs with sane defaults and idiomatic overrides | ✔ |

## Anti-Patterns

| Pattern | Description | Status |
|:-------:|:----------- |:------:|
| [Cascading Failures](/anti-patterns/cascading_failures.md) | A failure in a system of interconnected parts in which the failure of a part causes a domino effect | ✘ |
