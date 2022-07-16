# SharpNess
A Nes emulation in C#

## Introduction

SharpNess is a Nintendo Entertainment System Emulation built with .Net Framework 4.8.

## Usage

```run dotnet build``` to construct the executable  
```<path to executable>/Sharpness.exe``` to run the emulator

### Executable flags
-d : Debug Mode  
-g <path to .snes> : start with running a game  
-h : Show shelp  
-f : Open in fullscreen mode  

## Debug (TODO)
Add two projects:
- Debugger (Console App that shows memory addresses)
- SharpNess (Main emulator)
  - Add interrupt key to go forward one instruction at a time

## Test (TODO)
Unit test for 3 * 10 multiplication
- Assert that 
  - A register = $1E (30)
  - X register = $03 (3)
  - Y register = $00 (0)
  - $0000 address' first three bytes = [0A, 03, 1E]
