# Exit Reminder

An independent project to remind someone about a chosen item, such as a bottle or card, when they take their keys from their usual place by the door. The detection mechanism remains open.

## Status

Initial definition. No sensor, placement, or prototype has been validated.

## Initial scope

- Detect when the keys are taken from their usual place.
- Show the configured reminder in time to notice it before leaving.
- Return to the waiting state when the keys are put back.
- Avoid presenting an uncertain reading as fact.

Taking the keys is the proposed trigger for the pilot. The timing will be tested at the chosen location; a second exit sensor is not assumed.

## Technology map

| Area | Current direction | Status |
| --- | --- | --- |
| Key detection | Detect confirmed removal and return at the usual place by the door. | Required capability; sensor technology open. |
| Reminder interface | Show a configurable reminder locally before the person leaves. | Pilot direction; display or signal hardware open. |
| Connectivity | No network is required by the current pilot behavior. | Keep independent unless a concrete use case emerges. |
| Platform and power | Controller, firmware, mounting, and power source. | Open pending a test of the door and key area. |
| Documentation and localization | Living English specifications; English and Spanish product text. Use Lingui if a JavaScript/TypeScript interface is built. | Language direction agreed; Spec Kit and Lingui not installed. |

## Documents

- [Pilot specification](specs/001-keys-reminder/spec.md).
- [Shared method and architecture](docs/method.md).
- [Program coordination in Notion](https://app.notion.com/p/416504754f0881afaaa6e4297e39c813).

## Next decisions

Key location, sensor, alert type, power, and mounting. A central-display connection will be considered only if there is a clear use case.
