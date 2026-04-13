# Charge Runner - Codex Instructions

## Project goal
Build a small mobile-first Godot 4 portrait endless lane runner prototype.

## Core gameplay
- 3 fixed lanes
- player auto-runs forward
- player switches lanes left/right
- collectible dots fill a charge bar
- obstacles reduce progress or end the run
- a barrier appears at the end of each segment
- if charge is below the requirement, the run ends
- extra charge becomes bonus score

## Current priority
Build a greybox MVP with placeholder visuals only.

## Do not add yet
- ads
- in-app purchases
- polished art
- audio
- cosmetics
- multiple power-up types
- backend systems
- analytics

## Technical preferences
- Godot 4
- portrait orientation
- keep scenes and scripts small and readable
- prefer clear node names
- prefer simple exported variables for tuning
- keyboard input is acceptable for early testing
- touch support should be considered in structure

## File organization
- scenes go in `scenes/`
- gameplay scripts go in `scripts/`
- UI scenes/scripts go in `ui/`
- placeholder art goes in `assets/placeholder/`

## Working style
- make small, reviewable changes
- explain the plan before changing files
- summarize files changed after each task
- avoid broad refactors unless requested

## Git workflow
- Follow the branch strategy documented in `docs/workflow.md`
- Do not suggest direct work on `main`
- Keep changes scoped and suitable for feature branches