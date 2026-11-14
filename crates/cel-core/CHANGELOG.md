# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.5.2](https://github.com/nodeve-com/cel-core/compare/cel-core-nodeve-v0.5.1...cel-core-nodeve-v0.5.2) - 2026-11-14

### Other

- *(cel-core-nodeve)* release v0.5.1 ([#2](https://github.com/nodeve-com/cel-core/pull/2))

## [0.5.1](https://github.com/nodeve-com/cel-core/releases/tag/cel-core-nodeve-v0.5.1) - 2026-11-14

### Added

- fixes has inputs and field level completions
- add cel.block extension with slot-based variable binding
- resolve qualified proto message types as type values in evaluator
- add proto.hasExt and proto.getExt macro expansion
- add namespace and qualified identifier resolution
- add Any type semantic equality and map key numeric coercion
- add enum-to-int cross-type equality and comparison
- fix conversion operator edge cases for CEL conformance
- add base64.encode/decode runtime implementations
- add WKT value coercion and fix proto converter struct IDs
- add legacy enum mode with strong_enums flag
- add strong enum typing with EnumValue representation and constructors
- add two-variable macros, exhaustive comprehension eval, and map merge operator
- improve type checker inference with scoped type params and null assignability
- implement optional extension eval and optional chaining
- implement math extension eval and cross-type numeric comparison
- implement string extension eval and namespaced function dispatch
- improve proto message type conformance and WKT handling
- complete error-as-value semantics for logical operators
- add abbreviations support for namespace resolution
- add timestamp and duration evaluation support
- add CEL evaluation engine
- add proto type support and unified Ast type
- add extension library infrastructure

### Fixed

- *(checker)* a value beside null is nullable, and a nullable message selects
- *(checker)* select through a type parameter left unbound
- *(checker)* type an optional list element as its value type
- *(checker)* reject one type parameter bound to two value types
- *(checker)* keep a dyn type-parameter binding dyn
- build chrono without default features
- distinguish arity from type mismatches in function call errors
- report proper errors for macro calls with wrong argument count
- proto examples
- remove proto dev dep
- clippy issues
- type checking has statements

### Other

- release cel-core-nodeve from loom with release-plz ([#1](https://github.com/nodeve-com/cel-core/pull/1))
- name the fork's main crate cel-core-nodeve
- Merge fix/checker-select-type-param
- Merge fix/optional-list-literal-type
- *(checker)* a macro over an optional list element binds its value type
- *(checker)* pin the scope of incompatible type-parameter rejection
- Merge fix/checker-mismatched-type-params
- remove cel-core-lsp from workspace
- fmt
- bundle imports and fix dead code warnings
- initial api cleanup
- adds lsp snapshot tests
- more cleanup
- proto registry rename
- update handoff notes and docs for trait abstraction
- decouple prost/prost-reflect from cel-core via trait abstraction
- various readme and claude updates
- break down evaluator.rs into focused submodules
- claude stuff
- update roadmap, handoff, and conformance baseline
- adds time example and updates readme
- update README with ergonomic API examples
- add From/TryFrom traits for Value type conversion
- ast proto api
- update README with new crate structure and usage examples
- [**breaking**] consolidate internal crates into cel-core
- dep graph
- readme
