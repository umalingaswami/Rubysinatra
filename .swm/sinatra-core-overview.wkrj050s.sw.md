---
title: Sinatra Core Overview
---
# Sinatra Core Overview

Sinatra Core constitutes the foundational modules and classes that underpin the Sinatra framework. It encapsulates the main Sinatra module, which organizes essential functionalities such as routing, request processing, response generation, error handling, and middleware integration.

# Core Components

At the heart of Sinatra Core is the base application class from which all Sinatra applications inherit. This base class provides the structure for defining routes and handling HTTP requests. Additionally, Sinatra Core includes exception handling modules like `Sinatra::ShowExceptions`, which facilitate graceful error management by capturing exceptions during request processing and rendering detailed error pages, aiding development and debugging.

Utility classes such as `Sinatra::IndifferentHash` are also part of the core, offering flexible parameter handling by allowing access to hash keys using either strings or symbols. This enhances developer convenience and reduces common errors related to parameter access.

# Delegation and Middleware Support

Sinatra Core employs delegation patterns through modules like `Sinatra::Delegator` to simplify method calls and extend framework functionality. This design choice promotes cleaner and more maintainable code by abstracting method forwarding within the framework.

Middleware integration is seamlessly supported within Sinatra Core, enabling developers to insert custom or third-party middleware components into the request-response cycle. This extensibility allows for enhanced functionality such as logging, authentication, or session management without modifying the core application logic.

# Using Sinatra Core in Applications

Developers typically interact with Sinatra Core by extending or including its modules in their application classes. For example, by inheriting from the base application class, developers gain access to routing DSL and middleware support. Including modules like `Sinatra::ShowExceptions` during development helps in quickly identifying and resolving errors by providing detailed exception pages.

# Example: Exception Handling with Sinatra::ShowExceptions

The `Sinatra::ShowExceptions` module exemplifies Sinatra Core's approach to error handling. When included, it intercepts exceptions raised during request handling and renders a detailed error page instead of a generic server error. This feature is particularly useful in development environments to facilitate rapid debugging and improve developer experience.

&nbsp;

*This is an auto-generated document by Swimm 🌊 and has not yet been verified by a human*

<SwmMeta version="3.0.0" repo-id="Z2l0aHViJTNBJTNBUnVieXNpbmF0cmElM0ElM0F1bWFsaW5nYXN3YW1p" repo-name="Rubysinatra"><sup>Powered by [Swimm](https://app.swimm.io/)</sup></SwmMeta>
