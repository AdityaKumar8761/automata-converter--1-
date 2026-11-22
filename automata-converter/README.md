# Mealy ⇄ Moore Machine Lab

A browser-based Automata Theory mini-project built with vanilla HTML, CSS and JavaScript.

## Run
Open `index.html` in a modern browser. No dependencies, server, or installation required.

## Use
1. Choose Mealy or Moore mode.
2. Click **Load example** to try a ready-made machine, or add states.
3. Drag states to arrange them. Double-click a state to rename it (and set its output in Moore mode).
4. Choose **Connect states**, click a source and destination, then enter the transition symbols.
5. Use **Set initial** to mark the start state.
6. Click **Convert machine**, then use Next / Previous or Auto play to study the steps.

## Conversion notes
- Mealy → Moore creates a state for each distinct (destination state, transition output) pair, plus a fresh ε-output initial state.
- Moore → Mealy labels each transition with the output of its destination state. The initial Moore output has no corresponding Mealy transition.

This educational version expects a deterministic machine and does not perform completeness/equivalence checking. If a Moore state has multiple outgoing transitions with the same input, the diagram will still show them; determinism is the user's responsibility.
