# Recent developments

- new components
- pint for unit conversions
- debugging capabilities
- huge improvement in presolving
- (new) industry users
- exergy analysis -> https://github.com/oemof/exerpy

# Roadmap

## community

- time + funding
- get people involved in modeling, what are barriers?
- change time of online meeting
- frequent in person community meeting

## usability/applicability

- specialized component models + component models from datasheets
- model templates/ready to use models with an API
  - have prebuilt heat pumps, ORCs, refrigeration machines, etc.
  - repository for applications/models?
- document different classes of components and their nuances
- improve documentation on part load approaches
- graphical user interface -> no capacities

## education

- educational resources:
  - add references in docs
  - to complete https://github.com/IljaTuschy/tespy-znes-course
  - to complete https://github.com/fwitte/TESPy_teaching_exergy
  - to complete (minor changes) https://fwitte.github.io/intro-to-thermal-engineering/
  - csp systems: https://github.com/ddceruti/csp-exercises
  - ...?

## core topics

- some core changes: https://github.com/orgs/oemof/projects/5

- refactoring of fluid property wrappers: simplify addition of custom ones
- refactoring of guess values
- refactoring of solver:
  - isolation of subproblems (and solving them)
  - parallelize solving
  - automatically shutting off subproblems (e.g. bypassed components, shut down of subnetworks)
- refactor component and connection parameter setting/getting
  - clunky set_attr methods
  - storing parameters in dictionaries prevents IDEs to understand available attributes
- refactor connections/components:
  - replace component, "outX", other_component, "inX" with component.outlet, other_component.inlet
