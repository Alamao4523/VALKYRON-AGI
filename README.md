#  ⚜️ CERBERUS-AGI 2026 ⚜️

iOS On-Device UI Interaction Runtime (Research Project)

A long-running iOS interaction framework designed for persistent UI automation, testing, and research on jailbroken devices.

This project focuses on stability, low resource usage, and reliable on-device execution without requiring a permanent connection to a computer.

A demonstration video is available in VIDEO.mp4.

⸻

Overview

Most iOS automation approaches depend on external control (computer connection, simulators, WebDriver, etc.) or become unstable during extended runtimes.

This project explores a different approach:

Running a standalone interaction engine directly on the device, capable of operating for extended periods while remaining lightweight and resilient.

The system is distributed as a TrollStore IPA and supported by a small background helper component to improve reliability during long sessions.

⸻

Design Goals
	•	Extremely lightweight footprint (~20MB)
	•	Designed for very long runtimes (days/weeks)
	•	Standalone operation directly on the device
	•	Simple, reliable scripting model
	•	Low CPU and battery impact
	•	Resolution-agnostic interaction using OCR
	•	Integration with the native iOS Shortcuts app
	•	File-based IPC for robustness and simplicity

⸻

Core Capabilities
	•	Launch applications
	•	Read on-screen content using OCR
	•	Perform taps, swipes, and gestures
	•	Execute iOS Shortcuts
	•	Background execution designed for long sessions
	•	Script-driven interaction model
	•	Optional integration with external decision systems configured by the user

⸻

Operation Modes

Script Mode

Uses a simple proprietary line-based script format designed for reliability and ease of generation.

External Decision Mode (Optional)

External systems can be connected to interpret screen state and decide next actions. This is fully optional and user-configured.

⸻

Architecture
	•	TrollStore application
	•	Lightweight background helper for session stability
	•	File-based communication between components
	•	Designed to remain operational across common interruption scenarios
	•	Compatible with rootless jailbreak environments

⸻

Compatibility
	•	TrollStore
	•	Dopamine / Palera1n (rootless / roothide)
	•	iOS 15 / 16 / 17
	•	iPhone and iPad

⸻

Scripting Engine

The project uses a minimal custom scripting format where each line represents an action.
This avoids complex languages and improves reliability for extended runs.

An example script is included in the repository.

⸻

Resource Efficiency
	•	Near-zero CPU usage when idle
	•	Automatic memory recycling
	•	Designed for minimal battery impact

⸻

Intended Use

This project is intended for:
	•	UI automation research
	•	Long-duration interaction testing
	•	On-device experimentation with persistent UI control
	•	Research into resilient mobile automation techniques

⸻

Disclaimer

This is an independent research project exploring persistent on-device UI interaction on jailbroken iOS devices. It is not affiliated with Apple Inc.

Users are responsible for ensuring their usage complies with:
	•	Local laws and regulations
	•	The terms of service of any applications they interact with
	•	The rules of the jailbreak tools they choose to use

⸻

Contact

For research discussion or collaboration:

albertosendr@gmail.com

⸻

![unnamed](https://github.com/user-attachments/assets/a8f6b42e-8f09-45db-8369-86dbd7a838fe)

<img width="1045" height="896" alt="image" src="https://github.com/user-attachments/assets/fa8af2bb-b777-4a25-906e-bfbd7f72a0e0" />

