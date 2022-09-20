# Models

This module defines the model system for the office app suite. This represents a unified framework from which the applications can interact and extend one another, as well as provide extensions for each other. 

In general, this provides only generic models for applications - a very broad framework for conceptual scaffolding of parts within the applications. They are laid out as federated graph objects. Within each of the office applications, there are various models that are extended from these generic types.

The types are defined firstly in GraphQL and then transpiled to TypeScript. This is true for all applications. The resulting product is a federated graph structure, in accordance with Apollo's definition of federated graphs. The GraphQL client that serves requests from these applications to access data is the fantastic async-graphql crate from Rust. More details about the backend database structures are defined within the appropriate submodule.

More details about the generic model structure are laid out in MODELS.md.
