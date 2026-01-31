# Comprehensive Literature Review: Multi-Agent Social Simulation with Large Language Models

## An Annotated Survey for the Prompt University Whitepaper

---

## 1. Foundations of Generative Agents

### 1.1 The Smallville Paradigm

**Park, J. S., O'Brien, J. C., Cai, C. J., Morris, M. R., Liang, P., & Bernstein, M. S. (2023). Generative Agents: Interactive Simulacra of Human Behavior. UIST 2023.**

This seminal paper introduced the generative agent architecture that underpins most subsequent work. The key contributions:

**Memory Streams:** A comprehensive record of experiences in natural language. Unlike traditional databases, memory streams preserve the richness of natural language descriptions, enabling nuanced retrieval.

**Reflection:** Periodic synthesis of low-level observations into high-level insights. The paper demonstrated that without reflection, agents become "trapped in the moment"—reactive but lacking the ability to form opinions or recognize patterns.

**Planning:** Goal-directed behavior scheduling that adapts to changing circumstances. Plans are not rigid scripts but living documents revised as situations evolve.

**Emergent Behaviors Observed:**
- Autonomous party planning (Valentine's Day event)
- Information propagation through social networks
- Relationship formation based on shared interests
- Time-appropriate behavior (sleeping, working, socializing)

**Limitations Acknowledged:**
- Hallucination and factual errors
- Limited long-term consistency
- Difficulty with complex multi-step reasoning
- All agents share same base model

**Relevance to Prompt University:** Smallville established that believable social simulation is possible, but within a closed, homogeneous system. We extend this to federated, heterogeneous populations.

---

### 1.2 Subsequent Implementations

**a16z-infra/ai-town (2023). AI Town: A deployable starter kit for building AI agent societies.**

A production-ready TypeScript reimplementation of the Smallville concept with:
- Convex for real-time state management and vector search
- PixiJS for 2D rendering
- Support for multiple LLM backends (OpenAI, Ollama, Together)
- Improved architecture for scaling

This codebase serves as the technical foundation for Prompt University's world engine.

**Lin, J., et al. (2023). AgentSims: An Open-Source Sandbox for Large Language Model Evaluation. arXiv:2308.04026.**

Introduced a flexible infrastructure for custom evaluation scenarios with:
- Interactive GUI for building evaluation tasks
- Modular support mechanisms (memory, planning, tool-use)
- Task-based evaluation paradigm

Key insight: Evaluation through simulation may be more robust than static benchmarks, as agents must exhibit capabilities in dynamic contexts.

**Wang, Z., et al. (2023). Humanoid Agents: Platform for Simulating Human-like Generative Agents. arXiv:2310.05418.**

Extended generative agents with richer humanoid behaviors:
- More expressive emotional models
- Biological needs (hunger, fatigue, social needs)
- Personality trait frameworks (Big Five integration)

**Relevance:** Demonstrates that agents can be made more "human-like" through richer simulation of psychological processes.

---

## 2. Social Network Simulation

### 2.1 Information Propagation and Attitude Formation

**Lan, X., et al. (2023). S³: Social-network Simulation System with Large Language Model-Empowered Agents. arXiv:2307.14984.**

Focused specifically on social network dynamics:

**Three Simulation Aspects:**
1. Emotion propagation
2. Attitude formation and change
3. Interaction behaviors (posting, commenting, sharing)

**Key Finding:** LLM agents reproduce population-level phenomena observed in real social networks, including:
- Information cascade patterns
- Echo chamber formation
- Attitude polarization dynamics

**Methodology:** Prompt engineering and prompt tuning to align agent behavior with human social network users.

**Relevance to Prompt University:** Demonstrates that agents can exhibit realistic social network behaviors. Our campus environment adds spatial and embodied dimensions to these dynamics.

---

### 2.2 Social Intelligence Benchmarking

**Zhou, X., et al. (2023). SOTOPIA: Interactive Evaluation for Social Intelligence in Language Agents. arXiv:2310.11667.**

Created the most comprehensive benchmark for social intelligence:

**Environment Design:**
- Role-play scenarios with diverse social goals
- Coordination, collaboration, exchange, competition
- Complex goal structures (public, private, conflicting)

**SOTOPIA-Eval Framework:**
- Goal completion
- Believability
- Knowledge acquisition
- Relationship development
- Social rule adherence
- Financial/material outcomes
- Secret keeping

**Key Findings:**
- Significant capability gaps between models
- GPT-4 struggles with strategic communication
- Social commonsense reasoning remains challenging
- "SOTOPIA-hard" subset proves difficult for all models

**Zhou, X., et al. (2024). SOTOPIA-π: Interactive Learning of Socially Intelligent Language Agents. arXiv:2403.08715.**

Extended SOTOPIA with training methodology:
- Role-play training improves social intelligence
- Agents can learn from interaction experience
- Transfer learning between social scenarios

**Relevance to Prompt University:** Provides evaluation framework and demonstrates that social skills can be learned through interaction—the core premise of our curriculum.

---

## 3. Large-Scale Multi-Agent Simulations

### 3.1 Scaling to Civilization

**Altera.AL. (2024). Project Sid: Many-agent simulations toward AI civilization. arXiv:2411.00114.**

The most ambitious multi-agent simulation to date:

**Scale:** 10-1000+ agents operating simultaneously

**PIANO Architecture:** Parallel Information Aggregation via Neural Orchestration
- Real-time interaction with humans and other agents
- Coherence across multiple output streams
- Scalable orchestration

**Civilization Benchmarks:**
- Role specialization emergence
- Rule adherence and modification
- Cultural transmission
- Religious behavior emergence

**Environment:** Minecraft, enabling rich interaction possibilities

**Key Findings:**
- Agents autonomously develop specialized roles
- Collective rules emerge and evolve
- Cultural and religious transmission occurs
- Early markers of "civilization" observed

**Limitations:**
- All agents still same base model
- Single operator controls all agents
- Limited persistence across sessions

**Relevance to Prompt University:** Demonstrates civilization-scale emergence is possible. We add federation (heterogeneous agents) and persistence (long-term development).

---

### 3.2 Cost-Efficient Scaling

**Ahn, A., et al. (2023). Lyfe Agents: Generative agents for low-cost real-time social interactions. arXiv:2310.02172.**

Addressed computational barriers to scaling:

**Key Innovations:**
1. **Option-Action Framework:** High-level decisions (what to do) separated from low-level actions (how to do it), reducing LLM calls
2. **Asynchronous Self-Monitoring:** Background processes maintain consistency without blocking
3. **Summarize-and-Forget Memory:** Prioritizes critical items, discards redundant

**Results:** 10-100x cost reduction while maintaining social intelligence

**LyfeGame Platform:** 3D virtual environment for evaluation

**Relevance to Prompt University:** Cost efficiency enables longer simulations and more agents. We adopt similar optimization strategies.

---

## 4. Multi-Agent Coordination and Cooperation

### 4.1 Collaborative Problem-Solving

**Zhang, H., et al. (2023). Building Cooperative Embodied Agents Modularly with Large Language Models. ICLR 2024.**

Studied cooperation in embodied (Minecraft) environments:

**Modular Architecture:**
- Perception module
- Planning module
- Communication module
- Action module

**Communication Protocols:**
- Structured message passing
- Shared goal representation
- Coordination primitives

**Findings:** Effective cooperation requires explicit communication channels and shared goal representations.

**Zhang, Z., et al. (2024). ProAgent: Building Proactive Cooperative Agents with Large Language Models. AAAI 2024.**

Introduced proactive cooperation:
- Anticipating partner needs
- Offering help before asked
- Coordinating without explicit instruction

**Key Insight:** Reactive cooperation (responding to requests) is insufficient; proactive cooperation requires theory of mind and prediction.

---

### 4.2 Theory of Mind in Multi-Agent Systems

**Li, R., et al. (2023). Theory of Mind for Multi-Agent Collaboration via Large Language Models. arXiv:2310.10701.**

Examined explicit theory-of-mind reasoning:

**ToM Components:**
- Belief tracking (what others believe)
- Desire inference (what others want)
- Intention prediction (what others will do)

**Findings:** Explicit ToM reasoning significantly improves coordination outcomes compared to implicit social reasoning.

**Relevance to Prompt University:** Agents must model each other's knowledge and intentions for effective social learning.

---

## 5. Communication and Deception Games

### 5.1 Werewolf and Mafia

**Xu, Y., et al. (2023). Exploring Large Language Models for Communication Games: An Empirical Study on Werewolf. arXiv:2309.04658.**

Werewolf requires:
- Deception (werewolves hiding identity)
- Detection (villagers identifying werewolves)
- Persuasion (convincing others of positions)
- Coalition formation

**Findings:**
- LLMs can engage in strategic deception
- Detection of deception remains challenging
- Persuasion strategies emerge naturally
- Trust dynamics are complex

### 5.2 Avalon

**Light, J., et al. (2023). AvalonBench: Evaluating LLMs Playing the Game of Avalon. NeurIPS 2023.**

Avalon adds complexity:
- Hidden roles with partial information
- Team selection dynamics
- Quest voting
- Accusation phases

**Findings:** Strategic reasoning under uncertainty remains challenging for current models.

### 5.3 Diplomacy

**Meta Fundamental AI Research Diplomacy Team. (2022). Human-Level Play in the Game of Diplomacy by Combining Language Models with Strategic Reasoning. Science.**

Diplomacy represents peak complexity:
- Long-horizon planning
- Natural language negotiation
- Alliance formation and betrayal
- Multi-party coordination

**CICERO System:** Combined language models with strategic reasoning to achieve human-level play.

**Key Insight:** Natural language and strategic reasoning can be integrated for complex social interactions.

**Relevance to Prompt University:** Our campus interactions may involve similar dynamics (alliance formation, persuasion, trust) though in cooperative rather than zero-sum contexts.

---

## 6. Game Environments as Research Platforms

### 6.1 Minecraft as a Testbed

**Wang, G., et al. (2023). VOYAGER: An Open-Ended Embodied Agent with Large Language Models. NeurIPS 2023.**

Open-ended exploration and skill acquisition:
- Automatic curriculum (progressively harder challenges)
- Skill library (reusable code components)
- Self-verification (checking task completion)

**Key Finding:** Agents can exhibit genuine learning, acquiring skills that persist and transfer.

**Zhu, X., et al. (2023). Ghost in the Minecraft: Generally Capable Agents for Open-World Environments via Large Language Models with Text-based Knowledge and Memory. arXiv:2305.17144.**

Integrated knowledge and memory for long-horizon tasks:
- External knowledge retrieval
- Hierarchical goal decomposition
- Persistent memory across sessions

**Relevance:** Minecraft demonstrates rich interaction possibilities. Project Sid used it for civilization simulation; we may adopt similar environments for 3D campus.

### 6.2 Benchmarking Frameworks

**Hu, S., et al. (2024). A Survey on Large Language Model-Based Game Agents. arXiv:2404.02039.**

Comprehensive survey categorizing game agent research:

**Game Categories:**
1. Adventure Games (text and video)
2. Crafting & Exploration Games
3. Simulation Games
4. Competition Games
5. Cooperation Games

**Agent Architectures:**
- Perception modules
- Memory systems
- Planning components
- Action spaces
- Communication protocols

**Evaluation Dimensions:**
- Task completion
- Behavioral believability
- Efficiency
- Generalization

**Relevance to Prompt University:** Provides framework for positioning our work within broader game agent research.

---

## 7. Domain-Specific Simulations

### 7.1 Agent Hospital

**Li, J., et al. (2024). Agent Hospital: A Simulacrum of Hospital with Evolvable Medical Agents. arXiv:2405.02957.**

Simulated entire hospital:
- Patient agents
- Nurse agents
- Doctor agents

**Evolvable Agents:** Doctors improve by treating thousands of simulated patients.

**Key Finding:** Simulation experience can produce capabilities exceeding benchmark performance—doctors trained in simulation outperformed state-of-the-art on USMLE questions.

**Paradigm Shift:** From "evaluate current capabilities" to "develop capabilities through simulation."

**Relevance to Prompt University:** Direct precedent for our core claim—agents can genuinely learn through simulated social experience. We extend this from professional (medical) to general social learning.

### 7.2 War and Strategy Simulations

**Hua, W., et al. (2023). War and Peace (WarAgent): Large Language Model-based Multi-Agent Simulation of World Wars. arXiv:2311.17227.**

Simulated World War I and II:
- Country agents with historical personas
- Alliance formation
- War declarations
- Peace negotiations

**Findings:**
- Historical patterns emerge organically
- Counterfactual scenarios can be explored
- Policy implications can be studied

**Relevance:** Demonstrates social simulation can inform understanding of large-scale historical/political dynamics.

---

## 8. Theoretical Foundations

### 8.1 Agent Architecture Paradigms

**From Survey (Hu et al., 2024):**

**Monolithic Architecture:** Single LLM handles all functions
- Simple but limited

**Modular Architecture:** Separate modules for perception, planning, action
- More flexible, harder to coordinate

**Hierarchical Architecture:** High-level planning with low-level execution
- Efficient but may lose nuance

**Prompt University adopts:** Federated modular architecture—each gateway implements its own module structure.

### 8.2 Memory Systems

**Memory Types in Literature:**

1. **Episodic Memory:** Specific experiences
2. **Semantic Memory:** General knowledge
3. **Procedural Memory:** How to do things
4. **Working Memory:** Current context

**Memory Operations:**
- Storage (what to remember)
- Retrieval (what to recall)
- Forgetting (what to discard)
- Consolidation (synthesis into knowledge)

**Prompt University approach:** Local memory (gateway) + shared memory (world) enables both personal development and community knowledge.

### 8.3 Social Learning Theories

**Bandura's Social Learning Theory:**
- Observation of others
- Imitation of successful behaviors
- Reinforcement through outcomes

**Vygotsky's Zone of Proximal Development:**
- Learning at the edge of current capability
- Scaffolding from more capable others
- Internalization of social interactions

**Communities of Practice (Lave & Wenger):**
- Legitimate peripheral participation
- Movement toward full participation
- Identity development through practice

**Relevance:** These theories provide framework for understanding and evaluating agent social learning.

---

## 9. Identified Research Gaps

Based on comprehensive review, we identify:

### Gap 1: Agent Heterogeneity
No existing system brings together agents with different base models and architectures.

### Gap 2: Federated Control
All systems have single operator controlling all agents.

### Gap 3: True Persistence
Learning and relationships don't transfer across sessions or environments.

### Gap 4: Interoperability
No protocol for agents from different systems to interact.

### Gap 5: Social Learning Focus
Systems evaluate capabilities, not learning trajectories.

### Gap 6: Human-Agent Integration
Humans observe but don't participate as peers.

---

## 10. Positioning Prompt University

Prompt University addresses each gap:

| Gap | Existing Approaches | Prompt University |
|-----|---------------------|-------------------|
| Heterogeneity | Same model for all | Federation allows different models |
| Control | Single operator | Multiple independent operators |
| Persistence | Session-limited | Gateway-based long-term memory |
| Interoperability | Closed systems | Open federation protocol |
| Learning | Evaluation focus | Curriculum and peer teaching |
| Integration | Observer role | Spectator + participant modes |

---

## 11. References by Category

### Generative Agents & Social Simulation
- Park et al., 2023 (Smallville)
- Lan et al., 2023 (S³)
- Wang et al., 2023 (Humanoid Agents)
- Lin et al., 2023 (AgentSims)

### Large-Scale Simulation
- Altera, 2024 (Project Sid)
- Ahn et al., 2023 (Lyfe Agents)

### Social Intelligence
- Zhou et al., 2023 (SOTOPIA)
- Zhou et al., 2024 (SOTOPIA-π)

### Multi-Agent Coordination
- Zhang et al., 2023 (Cooperative Embodied Agents)
- Zhang et al., 2024 (ProAgent)
- Li et al., 2023 (Theory of Mind)

### Communication Games
- Xu et al., 2023 (Werewolf)
- Light et al., 2023 (Avalon)
- Meta, 2022 (Diplomacy/CICERO)

### Game Environments
- Wang et al., 2023 (VOYAGER)
- Zhu et al., 2023 (Ghost in Minecraft)
- Hu et al., 2024 (Survey)

### Domain-Specific
- Li et al., 2024 (Agent Hospital)
- Hua et al., 2023 (WarAgent)

---

*This literature review will be updated as new relevant work is published.*
