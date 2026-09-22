# Sustain-a-City

> A sustainable city-building simulation developed by a seven-person software engineering team using Godot and GDScript.

Sustain-a-City is a city-building game in which the player balances **pollution, income, electricity and city happiness** while developing a sustainable city. Buildings have different effects, become less effective over time and may require repair. External pollution also increases as the simulation progresses, so the player must continually adapt their strategy.

The project was developed iteratively across weekly sprints. Alongside gameplay development, the team practised requirements management, peer review, collaborative development and user-focused testing.

<p align="center">
  <img src="README_Assets\UI.png" width="90%" alt="Example Gameplay to Demonstrate UI">
</p>

## Technical Highlights

The project evolved from an initial minimum viable product into a playable simulation with interacting game systems and a user-facing feedback loop. The final game includes:

- **Dynamic city simulation** - data-driven building attributes affect pollution, income, electricity and happiness, with their effects changing over time.
- **Progressive difficulty** - external pollution increases as the game progresses, requiring the player to adapt their strategy.
- **Player feedback** - the Oracle provides context-sensitive messages, warnings and guidance based on the current state of the city.
- **Maintenance systems** - buildings and the city's air filter can be repaired as their effectiveness changes over time.
- **Scoring and game state** - the game records historical statistics, displays a sustainability score based on city performance and applies explicit pollution and financial lose conditions.
- **Construction and interaction** - buildings can take time to construct, can be inspected through tooltips and can be sold when permitted.
- **Interactive UI** - building menus, progress indicators, statistics, camera controls and end-of-game visualisations support the player throughout the simulation.

The implementation uses Godot scenes, autoloaded state, signals and reusable GDScript components to connect the simulation, UI and player actions.

## My Contribution

This was a seven-person group project, so the following describes my individual contribution rather than attributing the whole system to me.

I contributed across development, project coordination and documentation:

- **Gameplay systems:** paired with other developers to ramp up in Godot, then implemented and debugged interconnected stateful mechanics.
- **Simulation mechanics:** contributed to time-dependent building effects, yearly pollution progression, electricity and happiness calculations, income changes and game-state conditions.
- **Final feature development:** worked with a teammate on the Oracle feedback system, external pollution, air-filter repair functionality and associated UI behaviour.
- **Product Owner:** contributed to the initial product backlog and helped shape priorities in response to customer feedback.
- **Documentation Lead:** maintained project documentation and helped establish a process for collecting user-story test evidence.
- **Scrum Master:** coordinated a sprint and supported the team's development process.
- **Collaborative debugging:** investigated regressions and integration issues with teammates when changes to one system affected other parts of the game.

The project gave me experience moving from an unfamiliar framework to working directly on complex systems with shared state, time-dependent behaviour and multiple interacting UI outcomes.

## Software Engineering

This project was developed as a team rather than as an individual coding exercise. The process was deliberately structured around short feedback cycles and collaborative engineering practices.

### Agile Development & Requirements

- Worked in **weekly sprints** with defined sprint goals and a prioritised product backlog.
- Used **Jira/Kanban, user stories and acceptance criteria** to translate requirements into manageable development tasks.
- Used sprint reviews and customer/teaching-assistant feedback to refine requirements and reprioritise work.
- Updated user stories and tests when an implementation did not satisfy the original acceptance criteria, rather than treating the first implementation as final.
- Rotated roles including **Product Owner, Scrum Master and documentation lead**, giving the team experience across different aspects of project delivery.

### Collaborative Development

- Used **pair programming** and **mob programming** to solve technical problems, share knowledge and bring less-experienced developers up to speed with Godot.
- Used GitHub pull requests and peer review to coordinate changes and protect the shared codebase.
- Managed merge conflicts and coordinated larger changes through communication between developers and reviewers.

### Testing & Quality

- Created an autoloaded test runner that discovers and executes GDScript test files when the game launches.
- Used unit-style checks, manual acceptance testing and user-story evidence during development.
- Used failed checks, sprint reviews and peer feedback to identify incomplete requirements and revise features.
- Continued testing while integrating interconnected game mechanics, helping the team identify regressions when changes to one system affected another.

The repository currently contains a small automated smoke-test suite; broader testing was also carried out through user-story and manual acceptance testing during the project.

**Engine:** Godot 4.3  
**Language:** GDScript  
**Version Control:** Git / GitHub  
**Project Management:** Jira / Kanban  
**Development Practices:** Agile sprints, Scrum-style roles, pair programming, mob programming, pull requests, peer review, user-story testing

## Running the Game

The game is packaged for **Windows**.

### Installation

1. Download `Sustain-a-City.zip` from the [GitHub Releases](https://github.com/cjogilvy/Sustain-a-City/releases) page.
2. Extract the ZIP file.
3. Run `Sustain-a-City.exe`.

### Quick Start

Start a new game and build your city while balancing **pollution, income, electricity and happiness**. Buildings have different effects and become less effective over time, while external pollution increases as the simulation progresses.

For the full controls, gameplay instructions, system requirements and detailed explanations of the game's mechanics, see the **[Product Documentation](docs/Product_Documentation_Team_Teal.pdf)**.

## Documentation

The project is accompanied by detailed documentation containing both a **User Manual** and **Maintenance Guide**.

The documentation covers:

- System requirements and installation
- Controls and gameplay instructions
- Project structure and key Godot scenes/scripts
- Asset management and adding new buildings
- In-game systems such as the Oracle, repairs, time progression and scoring
- Win/lose conditions and statistics
- UI structure and building/exporting the game

This README provides the high-level overview; the documentation contains the detailed reference material for users and future developers.

- [Product Documentation](docs/Product_Documentation_Team_Teal.pdf)
- [Sprint Documentation](docs/Sprint_Documentation_Team_Teal.pdf)

## Project Context

Sustain-a-City was developed as **Software Engineering Coursework 2** by Team Teal. The project provided experience of developing a non-trivial software system collaboratively, from an initial MVP through iterative feature development, testing, documentation and integration.

The repository and accompanying documentation provide a fuller record of the team's implementation and development process.



