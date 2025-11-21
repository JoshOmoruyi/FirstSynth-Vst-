Introductory Synth VST

This project is an introductory software synthesizer built using C++ and the JUCE framework. It follows a tutorial-based foundation while allowing room for future customization and personal enhancements. Tweaks and improvements will be added over time to tailor the synth’s sound, interface, and workflow.

⸻

Frameworks
	•	JUCE — audio plugin framework for building VSTs, AUs, standalone synths, and more.

Language
	•	C++

⸻

Tutorial Reference

The original tutorial used to build the foundation of this synth can be found here:
https://www.youtube.com/watch?v=Ah4P-zOfdYc

⸻

Future Improvements
	•	UI and layout customization
	•	Additional oscillators or wave-shaping
	•	Filter and envelope adjustments
	•	Personalized presets
	•	Overall sound design enhancements
Build Instructions

✅ Prerequisites

Before building, install:
	•	JUCE (latest version): https://juce.com
	•	C++17-compatible compiler
	•	CMake (if using JUCE 7+)
	•	Plugin SDKs (see per-platform notes below)

⸻

Windows Build Instructions

Requirements
	•	Visual Studio 2022 (Desktop Development with C++)
	•	Windows 10/11 SDK (included with VS)
	•	VST3 SDK — JUCE includes it automatically

Steps
	1.	Clone or download the repository.
	2.	Open Projucer (inside your JUCE folder).
	3.	Open the .jucer project file (or generate one if using CMake).
	4.	Select your platform exporter:
	•	Visual Studio 2022 Exporter
	5.	Click Save and Open in IDE.
	6.	Build the project inside Visual Studio:
	•	Debug or Release
	7.	The compiled plugin will appear in:
/Builds/VisualStudio2022/x64/Debug/
/Builds/VisualStudio2022/x64/Release/

Plugin Install Location (Windows)

Copy the .vst3 file into
C:\Program Files\Common Files\VST3\
macOS Build Instructions

Requirements
	•	Xcode (latest)
	•	Command Line Tools
	•	VST3 + AU support (JUCE includes VST3; AU is built-in on macOS)

Steps
	1.	Open Projucer and load your .jucer file.
	2.	Add a macOS exporter:
	•	Xcode (MacOSX)
	3.	Click Save and Open in IDE.
	4.	Build in Xcode:
	•	Select MySynth - Standalone or MySynth - VST3
	5.	After compiling, the plugin appears in:
Builds/MacOSX/build/Debug/
Builds/MacOSX/build/Release/