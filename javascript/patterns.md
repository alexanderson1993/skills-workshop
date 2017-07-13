# Patterns

## Constructor

A function which returns an object. It can be simple as that, or it can be complicated by adding methods which can mutate that object and which can return data from that object in different ways (getters and setters)

## Singleton

A function which retains reference to an object after it is created. Then, when the object is needed, an enclosed function returns the reference to the object instead of creating a new one.

## Facade

An object which exposes an API which simplifies or obfuscates another API. JQuery and Polymer are excellent examples of this.

## Module

Cleanly separate concerns for an application into discrete pieces. Since blocks contain scope, it's possible to have multiple modules connected via an API or messages but that don't interact in any other way. Modules can have their own internal operations as well.

## Revealing Module

Similar to the module, but with an explicitly defined API, instead of implicitly defined.