# Specification 001: Reminder When Keys Are Taken

**Status:** proposal for validation. No sensor, mounting arrangement, or physical prototype has been verified.

## Purpose

Remind the person about an item they choose, such as a bottle or card, when they take their keys to leave the apartment.

## Use scenario

The keys rest in their usual place by the door. When they are taken, the object shows a configurable reminder that can be seen before leaving. When the keys are returned, it is ready for the next cycle.

## Initial behavior

1. **Waiting:** the keys are considered present and no exit reminder is active.
2. **Confirmed removal:** the configured reminder is shown once for that cycle.
3. **Keys absent:** the reminder does not repeatedly trigger while the keys remain absent.
4. **Confirmed return:** the alert is cleared and the system returns to waiting.
5. **Unknown state:** if detection is inconclusive, the system does not claim the keys are present or absent. How to display or record this uncertainty will be decided with the interface.

Taking the keys is the proposed pilot trigger; a second sensor for detecting exit is not assumed.

## Pilot acceptance criteria

- Confirmed removal activates the configured reminder without another action.
- Confirmed return resets the waiting state and allows a new cycle.
- The alert triggers once per cycle and does not repeat indefinitely while the keys remain away.
- Inconclusive readings are not counted as successful removals or returns.
- In a test at the chosen location, the alert can be noticed before the door is opened, and the object does not obstruct normal use of the keys or door.
- The test records removals, returns, and key movements that are not removals, along with successes, misses, and false alerts.
- The reminder and any user-facing status or error messages can be presented in English and Spanish. The same detected state and cycle behavior apply in either language.

## Out of scope for now

Tracking people, remotely locating keys, independently detecting door opening, and a central-display connection.

## Open decisions

- Usual key location and object placement.
- Detection method and treatment of ambiguous readings.
- Alert type, physical form, and power.
- Initial reminder content and how to configure it.
- Acceptable miss and false-alert rates after initial tests.
- How a person selects the display language and how a device without a JavaScript or TypeScript UI stores its translations.

## Evidence still needed

First, verify the use scenario and available space. Then compare sensors in a test setup and record the results. None of those tests has been performed yet.
