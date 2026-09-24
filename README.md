
# Cybersecurity Intrusion Detection Simulation

## Overview

This project is an **Agent-Based Cybersecurity Intrusion Detection Simulation** developed in **NetLogo** to model how cyber attacks propagate through a network and how defensive security mechanisms respond in real time.

The simulation represents a computer network consisting of servers, client nodes, attackers, and security defenders. Different attack types generate varying threat levels, while defensive agents attempt to detect, quarantine, and recover compromised systems.

The goal is to demonstrate core cybersecurity concepts such as:

* Intrusion Detection Systems (IDS)
* Firewall-based attack mitigation
* Malware and worm propagation
* Network defense strategies
* Threat monitoring and recovery mechanisms
* Agent-based modeling of cyber environments

---

## Features

### Network Topology

* Central server node representing critical infrastructure.
* Multiple client nodes organized in a layered network structure.
* Dynamic communication links between nodes.
* Visual representation of network status and security events.

### Multi-Type Attack Simulation

Three attacker categories are implemented:

| Attack Type | Threat Score | Description                                                          |
| ----------- | ------------ | -------------------------------------------------------------------- |
| Bot         | 1            | Low-level automated malicious traffic                                |
| Hacker      | 3            | Targeted intrusion attempts                                          |
| Worm        | 5            | Self-propagating malware capable of spreading across connected nodes |

Each attack contributes differently to the overall network threat level.

---

## Security Mechanisms

### Intrusion Detection System (IDS)

The IDS monitors network activity and probabilistically detects malicious behavior using a configurable detection accuracy parameter.

When an attack is detected:

* IDS alert is generated.
* Attack is blocked.
* Target node is quarantined.
* Security event is logged.

### Firewall Protection

Firewall rules provide an additional defense layer by intercepting attacks before they reach target systems.

### Autonomous Defender Agents

Defender agents continuously patrol the network and:

* Search for compromised nodes.
* Secure infected systems.
* Quarantine threats.
* Restore network stability.

---

## Attack Lifecycle

1. Attacker selects a target node.
2. Attacker moves toward the target.
3. Attack is launched.
4. IDS and Firewall evaluate the threat.
5. Attack is either:

   * Blocked and quarantined, or
   * Successfully breaches the target.
6. Defender agents respond.
7. Recovery mechanisms restore affected nodes.

---

## Worm Propagation Model

Worm attackers introduce additional complexity by spreading through network links.

When a worm successfully compromises a node:

* Neighboring connected nodes become potential infection targets.
* Infection spreads probabilistically.
* Additional breach events are recorded.
* Network-wide security degradation can occur.

This models real-world malware outbreaks and lateral movement behavior.

---

## Node States

Each network node can exist in one of three states:

| State       | Description                                           |
| ----------- | ----------------------------------------------------- |
| Normal      | Secure and operational                                |
| Compromised | Successfully breached by an attacker                  |
| Quarantined | Isolated after IDS detection or defender intervention |

Color-coded visualization allows real-time monitoring of node conditions.

---

## Metrics Tracked

The simulation continuously records:

* Total attacks launched
* Attacks blocked
* Successful breaches
* IDS alerts generated
* Threat level
* Suspicious activity score
* Bot traffic count
* Hacker traffic count
* Worm traffic count
* Network health percentage
* Number of compromised nodes
* Number of quarantined nodes

---

## Performance Indicators

### Detection Rate

Measures the percentage of attacks successfully blocked:

Detection Rate = (Blocked Attacks / Total Attacks) × 100

### Network Health

Measures the proportion of healthy nodes:

Network Health = (Normal Nodes / Total Nodes) × 100

### Threat Level

A dynamic score representing the current severity of malicious activity within the network.

---

## Recovery System

Compromised and quarantined nodes are assigned recovery timers.

After the timer expires:

* Nodes automatically return to normal operation.
* Labels and status indicators are reset.
* Network resilience can be observed over time.

---

## Technologies Used

* NetLogo 7.0.4
* Agent-Based Modeling (ABM)
* Cybersecurity Simulation
* Network Defense Modeling
* Intrusion Detection Concepts
* Malware Propagation Modeling

---

## Learning Outcomes

This project demonstrates:

* Agent-based simulation design
* Cybersecurity attack-defense modeling
* Network security concepts
* Intrusion detection workflows
* Malware propagation analysis
* Defensive response strategies
* Performance metric evaluation

---

## Future Improvements

Potential extensions include:

* Machine Learning-based intrusion detection
* Adaptive defender behavior
* Distributed Denial-of-Service (DDoS) attacks
* Advanced firewall rule sets
* Risk scoring systems
* Network segmentation strategies
* Security analytics dashboard
* Real-time threat intelligence integration



SETUP:

Download and install NetLogo
Open CYBERSECURITY INTRUSION DETECTION SIMULATION.nlogox in NetLogo
Use the interface controls to toggle Firewall and IDS on/off and run the simulation