# Traffic Light System for Four-Way Intersection

This traffic light system controls the flow of traffic at a four-way intersection with lights managing the following directions:
- **East-West Light**
- **West-East Light**
- **North-South Light**
- **South-North Light**
- **East-South Light**
- **South-East Light**

Each light operates in a sequence of **Red**, **Green**, and **Yellow** states with transitions based on a timer. The overall system follows a synchronized flow to ensure traffic moves safely through the intersection in each direction.

## Light Sequences and Transitions

1. ### East-West Light
   - **Red**: Initial state for stopping East-West traffic.
   - **Green**: Transition occurs when the timer expires, allowing East-West traffic to proceed.
   - **Yellow**: After the green phase, the light turns yellow, warning vehicles to prepare to stop.
   - **Transition**: After yellow, the light returns to red, allowing the East-South light to proceed.

2. ### West-East Light
   - **Red**: Initial state for stopping West-East traffic.
   - **Green**: Activates after the East-West light completes its cycle, allowing West-East traffic to proceed.
   - **Yellow**: Follows green, warning vehicles to slow down.
   - **Transition**: After yellow, transitions to red, allowing South-North light to proceed.

3. ### North-South Light
   - **Red**: Initial state for stopping North-South traffic.
   - **Green**: Activates after the West-East light, allowing North-South traffic to proceed.
   - **Yellow**: Follows green, indicating North-South traffic to prepare to stop.
   - **Transition**: After yellow, transitions to red, allowing East-South light to proceed.

4. ### South-North Light
   - **Red**: Stops South-North traffic.
   - **Green**: Activated after the North-South light, allowing South-North traffic to proceed.
   - **Yellow**: Follows green, warning vehicles to prepare to stop.
   - **Transition**: After yellow, transitions to red, allowing South-East light to proceed.

5. ### East-South Light
   - **Red**: Stops East-South traffic.
   - **Green**: Activates after the South-North light, allowing East-South traffic to proceed.
   - **Yellow**: Follows green, warning vehicles to slow down.
   - **Transition**: After yellow, returns to red, allowing West-East light to proceed.

6. ### South-East Light
   - **Red**: Stops South-East traffic.
   - **Green**: Activates after East-South light, allowing South-East traffic to proceed.
   - **Yellow**: Follows green, indicating South-East traffic to prepare to stop.
   - **Transition**: After yellow, returns to red, allowing East-West light to proceed.

## Flow Summary

The traffic light system operates in a coordinated manner, with each light switching to green in a sequence that allows traffic from each direction to proceed one at a time. Each green phase is followed by a yellow warning phase before turning red and allowing the next direction in sequence to proceed.

This sequence ensures:
1. Safe and orderly movement through the intersection.
2. Minimizes conflicts and potential collisions by controlling directional flows independently.
3. Supports a continuous and cyclic flow through the intersection, accommodating all directions.

The timer ensures that each phase (Red, Green, Yellow) completes before transitioning to the next phase, helping to control traffic effectively across the four-way intersection.
