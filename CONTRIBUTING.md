# Contributing

Thanks for taking a look at this project. Contributions of any size are welcome — bug fixes, documentation improvements, calibration notes, or wiring clarifications all help.

## Scope

This is a personal hobby project built around Raspberry Pi hardware. Keep changes focused and practical. Large rewrites or heavy abstractions are unlikely to be merged unless they solve a clear problem.

## How to contribute

1. Fork the repository
2. Create a feature branch: `git checkout -b fix/sensor-read-error`
3. Make your changes
4. Commit with a clear message (conventional style is appreciated):
   - `fix: handle BMP280 read failure gracefully`
   - `docs: clarify rain sensor wiring`
   - `feat: add mock mode for dashboard development`
5. Push and open a Pull Request

## Testing

- Changes to sensor code should be tested on a real Raspberry Pi when possible
- For UI-only work, you can stub sensor values in `app.py` temporarily — just do not commit mock data unless it is behind a dev flag
- Verify the dashboard loads at `/` and `/api/weather` returns valid JSON

## Code style

- Match the existing simplicity in `app.py` — no over-engineering
- Keep PRs small and scoped to one concern
- Comments only where the logic is not obvious

## Questions and bugs

Not sure where to start? [Open an issue](https://github.com/dogukannparlak/Weather-Station/issues) and describe what you are trying to do.
