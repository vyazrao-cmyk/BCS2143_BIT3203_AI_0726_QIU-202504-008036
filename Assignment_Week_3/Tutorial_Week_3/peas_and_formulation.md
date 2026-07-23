# PEAS and Formal AI Problem Formulation

<!-- Fill this in during/after tomorrow's tutorial, using your Part B and Part C answers
     from the Wk3b worksheet. Delete each instruction line once replaced with your own text.
     Everything below Part C is a preview for next week — a first sketch is fine, it does
     not need to be complete for the Concept Check. -->

## PEAS

**Performance measure (how success is judged):**
Reduce the time needed to find a parking space, provide accurate parking availability, and improve user satisfaction.

**Environment (where the agent operates):**
The university campus parking areas, including all parking lots and entrances.

**Actuators (how the agent acts):**
Displays available parking spaces on a mobile app, sends notifications, and guides users to the nearest available parking spot.

**Sensors (what the agent perceives):**
Parking occupancy sensors, CCTV cameras, GPS location, and parking database.

## Environment properties

<!-- Worksheet Part C. Circle/decide one option per line — this determines whether
     search or CSP fits your problem, which you'll formalise next week. -->

- Observable: partially 
- Deterministic:  no 
- Episodic or sequential: sequential
- Static or dynamic: Dynamic
- Discrete or continuous: Continuos

## State or variables
Current parking availability, user location, parking lot occupancy, and selected parking space.


## Initial state
The user enters the campus and requests a parking space through the mobile application.

## Actions or domains
Search for available parking spaces, recommend the nearest parking spot, update parking status, and notify users when parking availability chang

## Transition model or constraints
Parking availability changes whenever a vehicle enters or leaves a parking space. Users may not always choose the recommended parking space, and sensor updates may have slight delays.

## Goal test
The user successfully reaches and parks in an available parking space with minimal waiting time.

## Path cost
The total time taken to find and reach an available parking space, including travel distance.

## Heuristic, where applicable
Choose the nearest available parking space with the shortest estimated travel time.

---

## Appendix: draft simple reflex agent rules (early sketch, Part D)

<!-- Optional early thinking from the tutorial — condition-action rules, not the final
     algorithm. Keep or delete once your real AI method is decided next week. -->

- Rule 1 — if: an available parking space is detected then:  recommend that parking space to the user.
- Rule 2 — if: the selected parking space becomes occupied, then: search for another available parking space.
- Rule 3 — if: all parking spaces are full, then: notify the user and suggest the nearest alternative parking area.
