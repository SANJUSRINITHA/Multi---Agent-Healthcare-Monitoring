# Multi-Agent Healthcare Monitoring System

## About the Project

This project is a healthcare monitoring system built using a multi-agent approach. The main idea is to have different agents handle different monitoring and analysis tasks instead of depending on one single system to do everything.

The agents communicate with each other using a peer-to-peer approach and can work on different tasks in parallel. This helps the system process multiple health-related inputs at the same time and makes the overall architecture more distributed.

The project is mainly developed to explore how multi-agent systems and decentralized communication can be used for healthcare monitoring.

## How It Works

The system is divided into multiple agents, where each agent has a specific role.

For example:

- One agent can monitor patient vital parameters.
- Another agent can analyze the collected data.
- A risk assessment agent can check for abnormal conditions.
- An alert agent can generate notifications when a critical condition is detected.
- Agents communicate with each other through the peer-to-peer communication layer.

The agents can work simultaneously rather than waiting for one task to finish before starting another.

```text
Patient Data
     |
     +-------------------+
     |         |         |
     v         v         v
  Agent 1   Agent 2   Agent 3
  Monitor   Analysis    Risk
     \         |         /
      \        |        /
       +-------+-------+
               |
          Alert / Decision
