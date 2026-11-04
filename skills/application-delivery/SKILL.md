---
name: application-delivery
description: "Builds or extends a working application from requirements through implementation and verification. Applies to application delivery rather than agent architecture guidance alone."
---
<!-- coderabbit-ai-generated:v1 -->


# Application Delivery

<!-- coderabbit-ai-generated:v1 -->

<!-- coderabbit-ai-generated-section:v1:dd3a5295c2a83d91e4afb203afbb87c53b0c107fbbebd01f22e4cd6b4fefb4d2 -->

## When to Activate

Use to build an application, implement a feature, or repair a user-facing workflow. Do not activate for LLM pipeline architecture: use project-development; or for individual agent tool contracts: use tool-design.

<!-- /coderabbit-ai-generated:v1 -->

## Core Concepts

A working application is an end-to-end path through interface, state, and dependencies. Delivery requires evidence that the path works in its actual environment, including honest reporting of anything that could not be exercised.

## Practical Guidance

1. Inspect repository instructions, existing behavior, callers, tests, and setup. Define the user journey and acceptance conditions, preserving existing contracts unless a change is authorized.
2. Choose the smallest complete design that fits the stack. Identify state transitions, error and empty states, access boundaries, responsive behavior, and dependency integration where relevant.
3. Implement a usable vertical slice and extend it to the requested scope. Reuse established patterns; keep secrets out of source and avoid destructive changes to unrelated data.
4. Run the narrowest meaningful tests and required project checks. Start the app when feasible and exercise the affected flow, including failure states. For visual interfaces inspect the rendered page at appropriate viewport sizes.
5. Report the changed behavior, checks and remaining gaps. Do not deploy, publish, or modify external systems without authorization.

## Examples

For a search feature, verify input, loading, results, empty and failure states with representative data. For an API change, exercise callers and invalid input as well as the successful response.

## Guidelines

- Follow the repository's setup and testing procedures and preserve unrelated edits.
- Verify behavior at the boundaries changed, not just that the build compiles.
- Use realistic local fixtures and disclose unavailable services or untested paths.

## Gotchas

1. **Mock-only success**: A component test can miss a broken service boundary; exercise the integrated path when feasible.
2. **Invisible state**: Empty and failed requests need usable feedback, not a blank screen.
3. **Contract drift**: Updating tests to match an accidental interface change hides regressions; compare with existing callers and specifications.

## Integration

- project-development covers LLM pipeline shape and model fit.
- asset-production covers creation and export of visual assets.
- evaluation covers general quality gates and regression strategies.

## References

Use repository instructions, existing contracts, and the selected framework's documentation as appropriate.
