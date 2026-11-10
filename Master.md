ATOMIQ — Complete Master Development Prompt
ATOMIQ
Imagine. Instruct. Experiment.
THE INTERACTIVE VIRTUAL SCIENCE LABORATORY









nis.edu.kz


Interactive simulations
AI-assisted learning
Scientific accuracy


PART 1 — Your role and overall mission
You are a senior software architect, full-stack developer, scientific simulation engineer, UI/UX designer, AI integration engineer and technical project manager.

Your task is to design and develop AtomIQ, a complete, sophisticated, browser-based virtual science laboratory.

AtomIQ must allow users to:
- Build experiments by dragging and dropping scientific equipment.
- Connect apparatus and components.
- Perform interactive experiments.
- Observe scientific phenomena through visual simulations.
- View equations, calculations, measurements and observations.
- Ask an AI science assistant questions and give it commands.
- Learn scientific concepts through experimentation.
- Create and save their own experiments.
- Explore experiments created by the AtomIQ team and, eventually, the community.
The central principle: AtomIQ must actually simulate science. It must not merely describe what would happen.

For example, if a chemical reaction produces gas, users should see bubbles forming and rising. If a solid is consumed, it should visibly change. If heat is released, the simulation should visually communicate the temperature increase. The observation table should show the corresponding scientific observations.

Do not build a collection of static illustrations pretending to be simulations.
PART 2 — Brand identity and visual direction
Brand name: AtomIQ

Tagline: Imagine. Instruct. Experiment.

Brand personality:
- Scientific and sophisticated.
- Intelligent and modern.
- Professional but welcoming.
- Innovative without unnecessary visual complexity.
- Suitable for students, educators and independent learners.
Colour system
Colour	Hex	Purpose
Electric Blue	#36BDF5	Primary actions and highlights
Scientific Violet	#8B7CF6	AI and advanced features
Deep Navy	#111827	Dark theme backgrounds
Cloud White	#F4F7FB	Light theme backgrounds

Use a carefully designed light and dark theme. Maintain readability, contrast, visual hierarchy and consistent component styling.

The logo direction should use a scientific symbol above the AtomIQ wordmark. The wordmark should be prominent, with an appropriately designed bulb-inspired detail in the IQ portion, following the approved concept. Do not redesign the brand arbitrarily.
PART 3 — Technology architecture
Build AtomIQ as a modern web application.
Area	Preferred technology
Frontend	React + TypeScript
Build system	Vite
Styling	Tailwind CSS
2D graphics	SVG, Canvas
3D graphics	Three.js where genuinely useful
Physics calculations	TypeScript scientific engines and solvers
Backend and database	Supabase
Database	PostgreSQL
Authentication	Supabase Auth
Private files	Supabase Storage
Server-side operations	Supabase Edge Functions or secure backend services
AI assistant	Grok API through a secure backend
Version control	GitHub
Deployment	Static frontend hosting plus separately hosted backend

Use TypeScript throughout the main application. Python may be used for small development utilities, preferably under 150 lines, but not as the runtime simulation engine.
Architecture principles
Separate the application into:
1. User interface.
2. Equipment and workspace management.
3. Scientific simulation engines.
4. Reaction and experiment knowledge base.
5. AI communication layer.
6. Authentication and user data.
7. Community and publishing.
8. Administration and request management.
Do not put all application logic into one enormous component or file.

Keep the frontend, backend, simulation engines and database responsibilities clearly separated.

Supabase stores approved scientific definitions and application data. It does not perform the physical simulation itself.

AtomIQ's own simulation engines perform calculations, validate actions and render the visual results.
PART 4 — Complete website structure
Create a polished, responsive website with the following permanent sections.
Main website pages
1. Home
2. Dashboard
3. Explore Experiments
4. Physics Studio
5. Chemistry Studio
6. Biology Studio
7. Anatomy Studio
8. Earth & Space Studio
9. Your Lab
10. AtomIQ Intelligence
11. Learning Centre
12. Community
13. Published Experiments
14. User Profile
15. Settings
16. About AtomIQ
17. Contact Us
18. Privacy Policy
19. Terms and Conditions
20. Login, registration and account recovery
These should be real application pages with appropriate routing, not merely buttons that open unfinished placeholders.
Homepage
The homepage should introduce AtomIQ and its capabilities.

Include:
- A strong hero section with the AtomIQ brand.
- A clear explanation of the virtual laboratory.
- Direct access to the studios.
- Featured experiments.
- Interactive experiment previews where available.
- An introduction to AtomIQ Intelligence.
- Learning and community sections.
- A clear call to action to start experimenting.
Avoid excessive text, unnecessary animations and clutter.
Dashboard
The dashboard should provide:
- Recently opened experiments.
- Saved experiments.
- Continue experimenting.
- Recommended experiments.
- Learning progress.
- Recent community updates.
- Quick access to each studio.
Only display information that is genuinely available to the logged-in user.
PART 5 — Universal laboratory workspace
All studios should use a consistent, adaptable workspace.








blink.new


Workspace layout
A. Left panel — Equipment Library

Contains:
- Equipment search.
- Expandable equipment groups.
- Equipment cards or icons.
- Short descriptions.
- Drag-and-drop support.
B. Centre — Experiment Canvas

This is the main working area.

It should support:
- Dragging and dropping equipment.
- Moving and arranging objects.
- Selecting objects.
- Connecting compatible components.
- Zooming and panning.
- Rotating where appropriate.
- Deleting and duplicating.
- Selecting multiple objects.
- Snap-to-position and alignment.
- Visual feedback when components are connected or incompatible.
C. Right panel — Properties and AtomIQ Intelligence

When an object is selected, display relevant properties such as:
- Name.
- Scientific properties.
- Dimensions or values where applicable.
- Editable parameters.
- Connections.
- Simulation status.
The AI assistant should also be accessible from this area.

D. Bottom panel — Scientific Results

Provide a flexible panel for:
- Measurements.
- Equations.
- Observations.
- Calculations.
- Graphs.
- Reaction results.
- Experiment logs.
The bottom panel should not unnecessarily obstruct the canvas. Users should be able to expand, collapse and resize it.

E. Top toolbar

Include:
- Save.
- Undo.
- Redo.
- Run.
- Pause.
- Reset.
- Fullscreen.
- Experiment name.
- Simulation status.
All controls must perform their actual advertised functions.
PART 6 — Equipment library and workspace navigation
This is an important navigation requirement.
Distinguish subjects from equipment groups
Physics has separate subject workspaces:
- Electricity
- Magnetism
- Optics
- Mechanics
- Waves
- Thermodynamics
- Gravity
- Modern Physics
The navigation hierarchy must be:

Physics → Electricity → Equipment Groups → Individual Equipment

Selecting Electricity opens the Electricity workspace.

Within Electricity, the equipment groups are expandable sections—not separate workspaces.
Expandable equipment groups
Use the same equipment-library behaviour throughout all studios.

Users must be able to:
- Expand and collapse multiple groups.
- Keep several groups open simultaneously.
- Drag equipment from different groups onto the same canvas.
- Search across all groups in the current studio.
- Continue using existing canvas objects while browsing other groups.
Searching, expanding and collapsing groups must never clear the canvas or change the workspace.
Studio group definitions
Electricity
- Power Sources
- Circuit Components
- Wires & Connections
- Measuring Instruments
- Electrical Devices
- Advanced Components
Magnetism
- Magnets
- Magnetic Materials
- Magnetic Field Tools
- Compasses
Chemistry
- Chemicals
- Glassware
- Indicators
- Reaction Tools
- Laboratory Tools
All Chemistry groups must remain available within one integrated Chemistry workspace.

Biology
- Cells
- Microscopes
- Slides
Anatomy
- Organs
- Human Body Systems
Earth & Space
- Stars
- Planets
- Moon
- Asteroids
Additional relevant groups may be added as the equipment library expands.
Workspace preservation
When switching between major studios:
- Preserve the previous workspace as a recoverable draft.
- Never silently delete unsaved experiments.
- Provide an Undo or recovery option.
- Keep saved experiments safe.
- Restore the previous workspace when the user returns.
Changing an equipment group must not be treated as switching studios.
PART 7 — Physics Studio
Physics must provide real interactive calculations and visual simulations.
7.1 Electricity
Build a circuit simulator with:
- Batteries and power supplies.
- Cells.
- Resistors.
- Bulbs.
- LEDs.
- Switches.
- Motors.
- Buzzers.
- Fuses.
- Ammeters.
- Voltmeters.
- Wires and connectors.
- Other relevant electrical components.
Required functionality:
- Drag-and-drop components.
- Easy wire joining.
- Connection snapping.
- Junctions and branches.
- Series and parallel circuits.
- Open and closed circuits.
- Voltage, current and resistance calculations.
- Power calculations.
- Real-time measurement displays.
- Circuit diagrams.
- Fault detection.
- Graphs where appropriate.
Use a proper circuit-solving engine, such as Modified Nodal Analysis (MNA), rather than hardcoded answers.

The solver must be tested against known circuits.

Wire joining must be intuitive. Do not require users to make extremely precise mouse movements to connect components.
7.2 Magnetism
Implement:
- Bar magnets.
- Strong and weak magnets.
- Magnetic materials.
- Iron filings.
- Compasses.
- Magnetic field visualisation.
- Magnet-to-magnet interactions.
Requirements:
- Attraction and repulsion must depend on pole orientation.
- Magnetic strength must decrease realistically with distance.
- Iron must not be attracted from an unrealistic distance.
- Different magnetic materials must behave appropriately.
- Magnetic field lines should respond to the arrangement of magnets.
7.3 Optics
Implement:
- Mirrors.
- Lenses.
- Prisms.
- Glass slabs.
- Light sources.
- Walls and screens.
- Targets.
Show:
- Reflection.
- Refraction.
- Dispersion.
- Image formation.
- Ray paths.
- Angle measurements.
7.4 Mechanics
Include:
- Ramps.
- Blocks.
- Masses.
- Forces.
- Springs.
- Pulleys.
- Friction.
- Gravity.
Show actual motion and relevant measurements.
7.5 Waves
Include:
- Wave sources.
- Frequency.
- Amplitude.
- Wavelength.
- Reflection.
- Interference.
- Standing waves.
7.6 Thermodynamics and gravity
Include:
- Heat transfer.
- Temperature changes.
- Expansion.
- Cooling.
- Heating.
- Gravity.
- Orbital motion where supported.
Do not present unsupported calculations as scientifically accurate.
PART 8 — Chemistry Studio: visual reaction simulation
Critical requirement
Chemistry must be a genuine visual simulation environment.

A chemical equation appearing on the screen is not a completed simulation.

The user must be able to place a beaker, add chemicals, start a reaction and see the reaction progress visually.
8.1 User interaction
Example workflow:
1. User drags a beaker onto the canvas.
2. User adds hydrochloric acid (HCl).
3. User adds zinc (Zn).
4. AtomIQ identifies the reactants and relevant conditions.
5. AtomIQ checks Supabase for a scientifically approved reaction record.
6. Supabase returns the approved record.
7. AtomIQ validates the reaction and simulation conditions.
8. AtomIQ's Chemistry Engine performs the simulation.
9. The user sees the visual reaction and the corresponding scientific results.
For this example, the approved balanced equation is:
\[
Zn + 2HCl \rightarrow ZnCl_2 + H_2
\]

The simulation should show:
- Zinc pieces gradually becoming smaller.
- Gas bubbles forming around the zinc.
- Bubbles rising through the liquid.
- Hydrogen gas production being represented.
- Temperature behaviour consistent with the approved reaction model.
- The reaction progressing over time.
- The final products and observations.
The reactants must not simply disappear and get replaced by a final equation.
8.2 Supabase is the reaction knowledge base
Supabase must contain scientifically reviewed and approved reaction records.

Each reaction record should include at least:
Field	Purpose
Reaction ID	Unique identifier
Reactants	Required substances
Products	Resulting substances
Balanced equation	Scientifically balanced equation
Reaction type	Single displacement, precipitation, etc.
Conditions	Relevant concentration, temperature and other conditions
Observations	Approved scientific observations
Visual behaviour	Effects the simulator should display
Simulation parameters	Relevant model parameters
Approval status	Draft, under review, approved or rejected
Scientific reference	Supporting scientific source
Reviewer and date	Verification record

Include reaction matching rules that consider conditions, not just chemical names.

A reaction must not be executed as verified unless its record has been scientifically reviewed and approved.
8.3 Balanced equations
The balanced chemical equation must be stored in Supabase.

AtomIQ must:
- Retrieve the approved equation.
- Display it in the Chemistry Studio.
- Display it in the Observation Table.
- Use the same equation in the experiment results.
- Never independently invent or alter the approved equation.
If a reaction has no approved record, do not display a guessed equation as confirmed.
8.4 Visual reaction behaviour
The visual simulation engine must support reaction-specific behaviour.

10

Scientific event	Required visual effect
Gas formation	Bubbles form and rise
Solid consumption	Solid gradually shrinks or dissolves
Precipitation	New solid particles form
Colour change	Liquid changes colour
Heat released	Beaker develops a red-orange hot appearance
Heat absorbed	Visual cooling effect
Combustion	Appropriate flame or glow effect
Light production	Visible light emission
Vapour production	Appropriate vapour effect
Vigorous reaction	Faster, more intense visual changes where justified

The effects must be based on the approved reaction's actual properties.

Do not use the same generic animation for every chemical reaction.
8.5 Heat and temperature effects
When a reaction releases heat:
- Increase the simulated temperature according to the model.
- Give the beaker an appropriate red-orange hot appearance.
- Add subtle heat shimmer above the liquid where appropriate.
- Make the effect reflect the simulated temperature.
When a reaction absorbs heat:
- Show the appropriate cooling effect.
- Update the temperature measurement.
The visual effect and temperature measurement must remain synchronized.
8.6 Vigorous reactions and special visual events
Some reactions require more dramatic visual representation.

For example, a sodium-water reaction may require an educational simulation of rapid reaction, gas formation, heat and possible ignition.

Where scientifically justified, support:
- Rapid bubbling.
- Bright flashes.
- Flame or glow effects.
- Vapour effects.
- Simulated pressure events.
- Appropriate vessel-failure animations.
These must be controlled educational simulations, not instructions for performing hazardous experiments in real life.

Do not exaggerate or invent effects simply to make a reaction look exciting.
8.7 Continuous reaction timeline
Every reaction should have a continuous simulation timeline.
1. Starting: Reactants and apparatus are visible.
2. Reaction begins: Initial visible changes appear.
3. Reaction progresses: Gas, solids, colour and temperature evolve.
4. Reaction completes: Final products and observations are displayed.
Run, Pause and Reset must control the scientific simulation and visual animation together.
8.8 Observation Table — one source of truth
Confirmed requirement
This is a strict architecture rule:

No reaction should have a separate, manually invented observation table. Its observation definitions must come from the same approved Supabase reaction record that drives its visual simulation.

The Observation Table must display:
- Balanced chemical equation.
- Reaction type.
- Reactants.
- Products.
- Approved observations.
- Temperature information where available.
- Gas production where applicable.
- Visible changes.
- Reaction status.
- Live simulation measurements and timestamps.
For example:
Observation	Result
Balanced equation	Zn + 2HCl → ZnCl₂ + H₂
Reaction type	Single displacement
Gas produced	Hydrogen
Visible change	Bubbles form
Solid change	Zinc gradually dissolves
Temperature	As recorded by the simulation
Final products	Zinc chloride and hydrogen

The exact approved observation definitions must come from Supabase.

AtomIQ may record:
- Timestamps.
- Simulation progress.
- Measured temperature.
- Calculated gas production.
- Other measured simulation values.
These live values must not modify the original approved scientific record.

The visual engine and Observation Table must be driven by the same reaction record and synchronized simulation events.

If bubbles are shown, the corresponding gas observation must be available in the table. If a solid is consumed, the table must show the corresponding observation. If the temperature changes, the table must reflect it.

The table must not claim an event that the simulation did not produce.
8.9 When a reaction is unavailable
AtomIQ must never assume that a reaction is impossible merely because it is missing from Supabase.

Display an official message such as:

Reaction Not Available

"We couldn't find a verified record for this reaction in the AtomIQ reaction library.

This may mean that the substances do not react under the specified conditions, or that this reaction has not yet been added to our library as AtomIQ is still under development.

Our reaction library is continuously expanding. You can explore other available experiments or suggest this reaction through Contact Us."

Distinguish three situations:
1. No known reaction under the specified conditions.
2. Reaction not currently available in the AtomIQ library.
3. More information is required to identify or validate the reaction.
Do not confuse an absent database record with proof that no reaction occurs.
8.10 Grok's role in missing reactions
Grok may help identify a potentially relevant reaction and explain what information is missing.

However:
- Grok cannot approve reactions.
- Grok cannot directly insert records into Supabase.
- Grok cannot execute an unapproved reaction.
- Grok cannot invent an equation and present it as verified.
A proposed reaction must pass scientific review before it becomes available in AtomIQ.
8.11 Initial Chemistry library
Build a structured library of scientifically reviewed reactions.

Start with approximately 15–20 carefully selected and verified educational reactions, rather than thousands of unverified records.

Each reaction must have:
- A balanced equation.
- Conditions.
- Products.
- Reaction type.
- Approved observations.
- Visual behaviour.
- Scientific references.
- Approval status.
Do not activate placeholder or fabricated reactions.
PART 9 — Biology Studio
Build an interactive Biology Studio with:
- Animal cells.
- Plant cells.
- Cell organelles.
- Microscopes.
- Slides.
- Biological specimens where supported.
Show:
- Cell structures.
- Organelle selection.
- Labels.
- Zooming.
- Microscopic views.
- Educational explanations.
Use accurate scientific diagrams and interactive representations.
PART 10 — Anatomy Studio
Include:
- Human body.
- Organs.
- Human body systems.
- Circulatory system.
- Respiratory system.
- Digestive system.
- Nervous system.
- Skeletal system.
- Muscular system.
Users should be able to select structures, explore their relationships and view explanations.

Keep the information educational and scientifically reviewed.
PART 11 — Earth & Space Studio
Include:
- Stars.
- Planets.
- Moon.
- Asteroids.
- Solar system.
- Orbits.
- Space phenomena.
Provide interactive visualisation of supported concepts such as:
- Planetary motion.
- Lunar phases.
- Orbital relationships.
- Scale comparisons.
- Gravity.
Clearly distinguish simplified educational models from physically precise simulations.
PART 12 — Your Lab
Your Lab is a flexible custom experiment-building environment.

Users should be able to:
- Select equipment from available libraries.
- Place objects on a canvas.
- Connect compatible objects.
- Change supported properties.
- Run experiments.
- Save and restore projects.
Include the approved categories:
- Electricity
- Light
- Chemicals
- Magnets
- Human Body
- Mechanics
- Cell Biology
Equipment should be modular and data-driven so new items can be added without rewriting the entire application.

Do not allow unsupported objects to pretend to have working simulation behaviour.
PART 13 — AtomIQ Intelligence: AI science assistant
AtomIQ Intelligence should be the intelligent assistant available across the laboratory.

Use Grok through a secure backend connection.

The AI should support:
- Text conversations.
- Voice conversations.
- Experiment planning.
- Scientific explanations.
- Equipment recommendations.
- Troubleshooting.
- Command interpretation.
- Learning support.
- Result interpretation.
- Experiment suggestions.
13.1 Strict responsibility boundary
Non-negotiable security rule
AtomIQ owns and controls the entire laboratory. Grok does not.

Grok must not directly manipulate:
- Equipment.
- Canvas objects.
- Equipment libraries.
- Databases.
- Simulation engines.
- Reaction records.
- Experiment execution.
Grok receives only the information AtomIQ deliberately sends.
13.2 Information sent to Grok
Send only:
1. Conversation context: Current request and relevant conversation history.
2. Canvas snapshot: Current equipment IDs, positions, connections, experiment state and relevant measurements.
3. Current category library: Available equipment, groups and capabilities within the currently selected category.
Do not automatically send every studio's equipment library.
13.3 Responsibility of Grok
Grok handles:
- Understanding natural language.
- Planning experiments.
- Explaining concepts.
- Diagnosing problems.
- Suggesting possible actions.
- Recommending experiments using available equipment.
- Identifying missing equipment.
- Explaining scientific results.
13.4 Responsibility of AtomIQ
AtomIQ handles:
- Equipment validation.
- Object placement.
- Canvas updates.
- Connections.
- Simulation calculations.
- Reaction execution.
- Measurements.
- Graphs.
- Observations.
- Saving and restoring.
- Action history.
- Permissions and security.
Grok returns structured suggestions and action proposals. AtomIQ validates every proposal against actual equipment IDs, permissions, scientific constraints and current state before executing it.

Never execute arbitrary code returned by Grok.
13.5 Intelligent command execution
Use a hybrid execution model.
Action	Behaviour
Simple, reversible command	Execute immediately if unambiguous
Medium-confidence command	Ask for clarification
Complex multi-step experiment	Show plan and request approval
Destructive action	Always request confirmation
Unsupported request	Explain limitation
Missing equipment	Identify missing requirement

Maintain action history and provide Undo wherever appropriate.
13.6 Voice interaction
Start with push-to-talk voice.

Requirements:
- Visible microphone indicator.
- Mute.
- Interrupt.
- End voice session.
- Clear distinction between listening and not listening.
- No background listening.
- Text and voice should share one conversation.
The assistant should have balanced initiative: offer useful suggestions without constantly interrupting.
13.7 AI memory
Make memory behaviour configurable and user-controlled.

Do not assume that all user conversations should become permanent memory. Provide clear controls over what is retained, and explain what is stored.
13.8 Language support
Support natural English and Hindi/Hinglish communication.

The assistant should understand common scientific terminology, informal commands and mixed-language questions.
13.9 Cost and API protection
- Keep API keys on the backend.
- Never expose the Grok API key in frontend code.
- Add rate limits.
- Add configurable usage limits.
- Monitor AI costs.
- Avoid unnecessary repeated requests.
- Allow the AI provider to be replaced in the future.
PART 14 — Missing equipment intelligence
AtomIQ must understand the difference between what a user wants to perform and what equipment is actually available.

Example:

A user asks Grok to perform an experiment requiring equipment that is not present in the current category library.

The correct workflow:
1. Grok identifies the experiment's requirements.
2. AtomIQ checks its actual equipment library.
3. AtomIQ identifies the missing equipment.
4. AtomIQ explains that the experiment cannot currently be performed in the available workspace.
5. AtomIQ offers scientifically suitable alternatives using existing equipment, if any exist.
6. AtomIQ provides a way to request the missing equipment.
Use this official message:
We're Still Growing!
This experiment requires equipment that is not currently available in AtomIQ.

AtomIQ is under active development, and we are continuously expanding our equipment library, experiments and simulation capabilities.

The required equipment may be added in a future update. In the meantime, you can explore the available experiments or request this equipment through our Contact Us page.

Do not promise a specific release date or claim that requested equipment has already been added.

Include a Request This Equipment action that opens the permanent Contact Us page with Equipment Request selected.

Never claim that unavailable equipment or functionality exists.
PART 15 — Learning Centre
Build an educational section that complements the interactive studios.

Include:
- Topic explanations.
- Experiment guides.
- Scientific concepts.
- Equations and definitions.
- Interactive demonstrations.
- Learning progress.
- Quizzes and practice activities.
- Links to relevant experiments.
Learning content should connect directly to the relevant studios.

For example, a lesson about Ohm's Law should link to the Electricity Studio and its circuit experiments.

Do not make the Learning Centre a disconnected collection of static articles.
PART 16 — Save, restore and experiment management
Users must be able to save experiments and return to them.

Implement:
- Save experiment.
- Save as a new experiment.
- Rename.
- Duplicate.
- Delete with confirmation.
- Restore previous saved versions where supported.
- Recently opened experiments.
- Experiment history.
- Autosave or recoverable drafts.
A saved experiment should preserve:
- Workspace and studio.
- Equipment IDs.
- Object positions.
- Connections.
- Configured properties.
- Simulation settings.
- Relevant experiment state.
- Observation and measurement history where appropriate.
Do not silently discard work when changing studios or navigating away.
PART 17 — Community
Build a Community section where users can discover and eventually share scientific work.

Include:
- Published experiments.
- Community updates.
- New equipment announcements.
- New reaction announcements.
- Bug-fix announcements.
- New simulation announcements.
- Experiment suggestions and discussions.
Community announcement workflow
Private requests and public announcements must remain separate.

Use this workflow:

Request received → Under review → Approved for development → Implemented → Tested → Public announcement

Only announce a feature as completed after it has actually been implemented and tested.

Example announcements:
- A new chemistry reaction has been added.
- Magnet attraction behaviour has been improved.
- A circuit connection issue has been fixed.
- New equipment has been introduced.
Do not expose private user submissions or email addresses in Community posts.
PART 18 — Permanent Contact Us page
Contact Us must be a permanent standalone website page.

It must be accessible from:
- Main navigation.
- Website footer.
- Missing equipment messages.
- Equipment request actions.
It must not be a popup-only form or temporary page.
Contact categories
Provide four categories:
1. Equipment Request
2. Bug Report
3. Experiment Suggestion
4. General Feedback
Form fields
- Category.
- Subject.
- Message.
- Optional email address.
Only collect information necessary for the user's chosen request.
Submission workflow
When a user submits a request:
1. Validate the form.
2. Store the submission securely in Supabase.
3. Send a notification to the owner's Gmail through a secure backend service.
4. Store the original request in private request records.
5. Make it available to the administrator for review.
The owner will supply the Gmail address during configuration.

Do not display the owner's email publicly.

Do not send automatic confirmation emails unless explicitly approved later.
Private request.md
Maintain a private, readable request.md record containing grouped submissions.

Its sections must be:
- Equipment Requests
- Bug Reports
- Experiment Suggestions
- General Feedback
Each entry should preserve:
- Unique request ID.
- Submission date.
- Subject.
- Original message.
- Optional email.
- Current status.
Similar requests may be grouped and their frequency counted, but individual original submissions must be preserved.

Important implementation rule: Supabase should be the source of truth. Generate or update the private request.md from database records. Do not use a publicly accessible frontend file or an unsafe shared-file overwrite process as the main storage mechanism.

Keep request.md and all request backups private. Never place them in the public GitHub repository or expose them through a public URL.
PART 19 — Permanent Privacy Policy page
Privacy Policy must also be a permanent standalone website page.

It must be accessible from the footer and other appropriate locations.

The policy must accurately explain:
- What information users voluntarily provide.
- Why that information is collected.
- How account and experiment data are handled.
- How Contact Us submissions are handled.
- What external services are involved.
- How AI requests are processed.
- Data retention.
- Security measures.
- User privacy rights.
- How users can contact AtomIQ about privacy.
User privacy principle
AtomIQ must not intentionally extract information from a user's phone or computer.

Do not introduce:
- Unnecessary device scanning.
- Unnecessary file access.
- Hidden data collection.
- Unnecessary device fingerprinting.
- Unnecessary analytics.
Only access information needed for the functionality the user deliberately uses.

Be accurate about technical limitations: hosting providers and security infrastructure may process limited technical information. Do not make misleading claims that no technical data is ever processed.
Proposed retention policy
Use data minimisation.
- Keep new requests while they are under review or in progress.
- Keep resolved requests for up to 12 months after resolution, then delete or anonymise them.
- Delete spam and accidental submissions when identified.
- Retain information longer only where legally required.
These are proposed operating rules and must be implemented consistently before the Privacy Policy claims they are in effect.

Do not create separate sections titled:
- "How Gmail and private request storage are used."
- "How changes to the policy are announced."
However, the actual data processing and legally necessary disclosures must still be transparently covered in the policy.

Because AtomIQ may be used by younger students, include appropriate privacy safeguards and obtain suitable legal review before public launch.
PART 20 — Supabase database architecture
Use Supabase for persistent, structured application data.

Create a properly designed schema for:
Table or data area	Purpose
profiles	User profiles
experiments	Saved experiments
experiment_versions	Version history
reaction_library	Approved reaction definitions
reaction_observations	Approved observation definitions
reaction_visuals	Visual simulation configuration
equipment_library	Equipment definitions
equipment_categories	Equipment groups and classifications
equipment_requests	User equipment requests
contact_requests	Contact form submissions
community_posts	Public announcements
learning_content	Learning materials
user_progress	Learning progress
simulation_records	Relevant experiment results
admin_activity	Administrative actions

This is a starting schema, not an instruction to create redundant copies of the same data.
Database principles
- Use proper relational design.
- Use foreign keys.
- Use validation constraints.
- Use timestamps.
- Use appropriate indexes.
- Use Row Level Security (RLS).
- Separate public content from private records.
- Protect administrative operations.
- Keep secret credentials on the backend.
Reaction records
The approved reaction record must be the source for:
- Balanced equation.
- Reaction type.
- Products.
- Conditions.
- Observation definitions.
- Visual simulation behaviour.
- Scientific verification.
AtomIQ must retrieve the same approved reaction record for both its visual simulation and Observation Table.

Do not create an independent hardcoded observation dataset in the frontend.
Supabase plan
Begin with the Free plan during development, but verify the current limits before launch.

Design the application so that it can be upgraded without major architectural changes.

Maintain separate private backups. Do not assume that the Free plan provides automatic database backups or permanent uptime.

Supabase is the data and backend platform—not the physics engine, chemistry engine or visual simulation engine.
PART 21 — Security and reliability
Security must be designed into the architecture.

Implement:
- Authentication and authorization.
- Supabase RLS.
- Server-side validation.
- Secure API endpoints.
- Rate limiting.
- Input sanitisation.
- Protection against unauthorized database access.
- Private storage for user requests.
- Safe error handling.
- Secure administrative access.
- Backup and recovery procedures.
Never:
- Expose API keys in frontend JavaScript.
- Trust AI-generated actions without validation.
- Allow Grok to write directly to the database.
- Allow unverified reactions to execute.
- Expose private request records publicly.
- Trust client-side permission checks alone.
PART 22 — Scientific accuracy and simulation quality
Scientific accuracy must take priority over visual excitement.

Every scientific engine should:
- Use documented equations and assumptions.
- Validate inputs.
- Handle invalid states.
- Display units.
- Use suitable numerical methods.
- Distinguish measured values from calculated values.
- Clearly identify simplified models.
- Include known-answer tests.
For complex phenomena that cannot be accurately simulated in the initial version, clearly state the limitation rather than pretending to have a complete simulation.

Maintain a scientific review process for the reaction library and educational content.
PART 23 — User experience and accessibility
The entire platform must be:
- Responsive on desktop, tablet and mobile.
- Comfortable to use with a mouse and touch input.
- Consistent across studios.
- Fast to navigate.
- Accessible by keyboard where practical.
- Clear about loading, errors and simulation status.
Use:
- Helpful tooltips.
- Clear equipment labels.
- Consistent icons.
- Contextual help.
- Confirmation before destructive actions.
- Useful empty states.
- Search with relevant results.
Avoid:
- Excessive popups.
- Overloaded sidebars.
- Tiny controls.
- Unnecessary animations.
- Hidden important actions.
- Inconsistent layouts between studios.
PART 24 — Testing requirements
Do not consider a feature complete merely because its interface looks finished.
Physics testing
- Test known electrical circuits.
- Verify voltage and current calculations.
- Test series and parallel connections.
- Verify magnetic force changes with distance.
- Test attraction and repulsion.
- Verify optics calculations and ray behaviour.
Chemistry testing
- Verify balanced equations.
- Check reaction matching.
- Check reaction conditions.
- Verify approved reaction records.
- Test each visual effect.
- Verify that the Observation Table uses the same approved record.
- Verify that live observations remain synchronized with the animation.
- Test unavailable-reaction handling.
- Confirm that unapproved reactions cannot execute.
AI testing
- Test simple commands.
- Test ambiguous commands.
- Test complex experiment plans.
- Test unsupported equipment requests.
- Verify that Grok cannot directly control AtomIQ.
- Verify that invalid action proposals are rejected.
- Test voice interruption and session controls.
Website testing
- Test authentication.
- Test save and restore.
- Test navigation.
- Test responsive layouts.
- Test Contact Us submissions.
- Test private request storage.
- Test administrator permissions.
- Test privacy controls.
- Test error recovery.
Maintain automated tests for important scientific calculations and application logic.
PART 25 — Development strategy and milestones
Do not attempt to build the entire platform in one uncontrolled coding operation.

Work in milestones.
1. Milestone 1 — Architecture and UI foundation
   
   Finalise architecture, routing, design system, responsive layout, authentication structure and universal workspace.
2. Milestone 2 — Equipment and workspace engine
   
   Build equipment libraries, expandable groups, drag-and-drop, canvas management, object properties, saving and recovery.
3. Milestone 3 — Physics engines
   
   Build Electricity, Magnetism, Optics, Mechanics and other initial physics simulations. Test calculations.
4. Milestone 4 — Chemistry engine
   
   Build reaction records, Supabase integration, reaction matching, balanced equations, visual effects, simulation timeline and synchronized Observation Table.
5. Milestone 5 — Other science studios
   
   Build Biology, Anatomy, Earth & Space and Your Lab.
6. Milestone 6 — AtomIQ Intelligence
   
   Integrate Grok, structured action proposals, context management, validation, text and push-to-talk voice.
7. Milestone 7 — Learning and community
   
   Build Learning Centre, experiment publishing, community updates and user progress.
8. Milestone 8 — Contact, privacy and administration
   
   Build Contact Us, private request records, Gmail notifications, Privacy Policy and administrative workflows.
9. Milestone 9 — Security and production readiness
   
   Complete testing, security checks, performance improvements, backups, documentation and deployment.
10. Milestone 10 — Collaboration
    
    Add real-time collaboration and shared experiments after the core platform is stable.

Approval process
Before starting each milestone:
1. Explain what will be developed.
2. List the pages, components and systems involved.
3. Identify dependencies.
4. Explain what will be tested.
5. Present the milestone plan for approval.
After approval:
- Implement that milestone.
- Test it.
- Fix identified issues.
- Report what is working.
- Report what is incomplete.
- Provide the files changed.
- Explain how to run and verify the work.
Do not silently skip milestones or claim that unfinished features are complete.
PART 26 — Deployment and GitHub
Use GitHub for version control.

Requirements:
- Organised repository.
- Clear folder structure.
- Meaningful commits.
- .gitignore.
- Environment variable examples.
- Setup documentation.
- Deployment instructions.
- No secrets committed to GitHub.
The frontend may be hosted on GitHub Pages or another static hosting provider, but Supabase and secure backend services must be hosted separately.

Do not assume GitHub Pages can securely execute server-side operations or protect API keys.

Provide a clear local development process and production deployment instructions.
PART 27 — Final delivery requirements
At the end of development, provide:
1. Complete source code.
2. Folder and file structure.
3. Database schema and migrations.
4. Supabase configuration instructions.
5. Environment variable template.
6. API and backend documentation.
7. Local setup instructions.
8. Deployment instructions.
9. Testing report.
10. Known limitations.
11. List of incomplete features.
12. Future development recommendations.
Every feature must be labelled honestly:
- Working: Implemented and tested.
- Partially working: Some functionality is implemented.
- Prototype: Demonstration only.
- Not implemented: Still requires development.
Do not label a simulated button, placeholder animation, hardcoded result or mock AI response as a completed production feature.

PART 28 — Final non-negotiable rules
These rules override convenience or shortcuts.
1. AtomIQ must be a real interactive virtual science laboratory.
2. Scientific simulations must show actual visual changes, not just written descriptions.
3. Supabase stores approved scientific definitions; AtomIQ performs the simulations.
4. The approved Supabase reaction record is the single source of truth for balanced equations, observations and visual reaction definitions.
5. The Observation Table must use the same approved reaction record as the visual simulation.
6. AtomIQ may add timestamps and measured simulation values without changing the original approved scientific record.
7. Unavailable reactions must be explained honestly. A missing record does not prove that no reaction exists.
8. Grok must never directly control equipment, canvas, libraries, databases or simulation engines.
9. AtomIQ validates and executes all AI action proposals.
10. Equipment groups are expandable sections, not separate workspaces.
11. Searching or switching equipment groups must never clear the canvas.
12. Contact Us and Privacy Policy must be permanent standalone pages.
13. Private user requests must never be publicly exposed.
14. Never claim that unimplemented features exist.
15. Never sacrifice scientific accuracy for visual effects.
16. Never expose secrets or API keys in the frontend.
17. Test every major feature before calling it complete.
18. Follow the milestone approval process.

PART 29 — Instructions before beginning development
Do not start writing code immediately.

First produce the following:
1. A complete technical architecture.
2. A detailed folder structure.
3. A page-by-page implementation plan.
4. The universal workspace design.
5. The equipment library architecture.
6. The Physics simulation architecture.
7. The Chemistry reaction and visual simulation architecture.
8. The Supabase database schema.
9. The AtomIQ Intelligence and Grok integration architecture.
10. The Contact Us, Privacy Policy and administration architecture.
11. A security plan.
12. A milestone-by-milestone testing plan.
Identify any conflicting requirements, technical limitations or missing decisions before implementation.

Wait for approval of the architecture and first milestone before writing production code.

The final goal is to create AtomIQ as a complete, expandable, scientifically reliable virtual laboratory—not merely a website with attractive science-themed graphics.

Final architecture principle
ATOMIQ owns the laboratory
AtomIQ Engine

Controls the canvas, equipment, calculations, simulations, observations and execution.


Grok Intelligence

Understands, explains, plans, diagnoses and suggests through controlled communication.


Supabase

Stores approved reactions, observations, equipment data, experiments and user records.


User Interface

Makes scientific experimentation intuitive, visual, interactive and accessible.



Imagine. Instruct. Experiment.