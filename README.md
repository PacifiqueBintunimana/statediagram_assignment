# Gishushu Traffic Lights System

## Overview

This project is a traffic light control system designed for the Gishushu intersection. The system uses six lights, each controlling traffic flow in a specific direction. Each light cycles through Green, Yellow, and Red states, with transitions triggered by timers.

## System Design

The traffic light system is structured as a state machine with the following components:

1. **Lights**: Each light represents a traffic direction (East-West, West-East, North-South, etc.).
2. **States**: Each light cycles through three states:
   - **Green**: Traffic can proceed.
   - **Yellow**: Warning state, indicating the light is about to turn red.
   - **Red**: Stop traffic.
3. **Timers**: Each state transition is controlled by a timer. When the timer expires, the light moves to the next state.

## Control Flow

- The system follows a sequence where each light passes control to the next light upon transitioning to Red.
- The sequence avoids conflicts by ensuring that opposite-direction lights are never Green at the same time.

## Recommendations

- Adjust timer durations based on traffic patterns.
- Consider adding sensors to adjust timers dynamically.
- Regular maintenance checks are recommended to ensure system reliability.

## Setup and Usage

1. **Configuration**: Set the initial timer durations for each light state.
2. **Deployment**: Install the system at the Gishushu intersection.
3. **Monitoring**: Use the provided interface to monitor light statuses and detect any issues.

---

This README provides a basic understanding of the traffic light system, including setup instructions and recommendations for optimal use.
