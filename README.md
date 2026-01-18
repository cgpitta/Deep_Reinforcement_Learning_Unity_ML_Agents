Abstract

AI in video games is a long-standing research area because video games are the perfect environment for AI research. Video games provide interesting and complex problems for agents to solve, virtual environments are safe and controllable, game environments provide an infinite supply of useful data for ML algorithms, and they are much faster than real-time. On the other hand, AI has been helping games to become better in the way we play, understand, and design them. Deep Reinforcement Learning is tailor made for creating adaptive and responsive agents in video games. 

While much reinforcement learning research focuses on algorithmic improvements, practical deployment requires understanding how training configurations impacts agent performance and behavioral diversity. This project systematically explores the hyperparameter space of Proximal Policy Optimization in game environments - investigating how learning rate, exploration parameters, and reward architecture influences how quickly agents can successfully learn to navigate environments and obstacles to achieve a goal. 

Problem Statement

Hyperparameters such as learning rate and entropy coefficient (beta) critically influence reinforcement learning performance by controlling how agents explore environments and update their policies. Reinforcement learning agents are highly sensitive to these choices, even slight variations can produce dramatically different convergence speeds and final performance. Poorly tuned hyperparameters can slow learning, cause training instability, and yield suboptimal policies.

Despite their importance, hyperparameter optimization in reinforcement learning remains challenging due to limited guidance on which parameters matter most for different task types. This project investigates hyperparameter sensitivity across two Unity ML-Agents environments of varying complexity: Hallway (simple, single-stage navigation) and Pyramids (complex, multi-stage manipulation with curiosity-driven exploration). Through systematic experimentation, we identify environment-specific tuning strategies and discover a novel requirement for asymmetric learning rates in dual-reward architectures.

Introduction

Non-Player Characters (NPC) have long served as the cornerstone of video games. They are vital to storytelling and creating immersive experiences within virtual worlds. When a non-player character (NPC) flanks you in a shooter-game or suddenly appears repeating random endless phrases and walks in endless circles, it isn’t “thinking”. It follows a flowchart and executes a prewritten script or traversing a behavior tree created by a designer who painstakingly anticipated every possible scenario. While this approach is reliable, it is also brittle. If the player did something that a designer didn’t anticipate, the illusion breaks. The NPC runs into a wall, gets stuck in a corner, or stands still while you snipe it. 

Deep Reinforcement Learning and tools like Unity ML-Agents are shifting the paradigm away from rigid, scripted behaviors to learned behaviors which provide players with dynamic and engaging experiences that evolve and adapt alongside their actions. 
