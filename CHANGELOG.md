# Changelog

All notable changes to ClearPlan InfraMapper are documented here.

## [v1.0.2] — 2026-06-26
- Fix roadmap sidebar drag-to-reorder: dragging the upper of two adjacent
  rows downward was a no-op (insert-before-target semantics); now detects
  top/bottom half of the drop target so both directions work for upgrade
  targets and manual tasks alike
- Future State nodes are now draggable with the same snap-to-alignment
  behavior as Current State; custom positions persist in JSON save/load
- "Show replaced systems" toggle lists original system names under the
  "Replaces N" badge on consolidated future nodes; "Reset Layout" button
  reverts to auto-computed positions
- Current and Future State track independent zoom/pan, restored
  separately when switching views
- Node card text (name, category, upgrade badge, connections) now uses
  real text measurement for truncation instead of a fixed character
  count, so it fills the available card width
- Added SECURITY.md, GitHub Pages hosting, and automated GitHub Release
  notes generation from this changelog on tagged pushes

## [v1.0.1] — 2026-06-17
- Test release to verify in-app update notification routine

## [v1.0.0] — 2026-06-17
### Initial Release
- Network diagram with Cytoscape.js, SVG node cards, categories, connections
- 200k+ icons via Iconify API; custom logo upload per node
- Future State view computed from upgrade targets
- Gantt roadmap: swimlanes, drag/resize bars, auto-phasing, deadline markers
- Manual (non-node) roadmap tasks with dashed-bar styling
- Category/swimlane color management from both Network Diagram and Roadmap views
- PNG and multi-page PDF export for both views
- JSON save/load; localStorage auto-save; full undo/redo
- Light, Dark, High Contrast, and Custom themes
- In-app update checker against GitHub releases
