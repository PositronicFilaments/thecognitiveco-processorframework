# Cognitive Co-Processor Workflows

## Workflow 1: Spatializing Agent Tasks
1. Identify all parallel agent tasks in the current scope.
2. Map each task to a specific quadrant in the visual workspace (VSCode logic maps).
3. Establish a "Spatial Anchor" (e.g., a specific file path or visual tag) for each task.
4. Monitor state changes relative to these anchors rather than through a linear log.

## Workflow 2: Externalizing Working Memory (Soil Commit)
1. Before context-switching, identify all "volatile" data currently in Mental RAM (e.g., specific variable names, local state logic).
2. Commit this data to a structured markdown file or DuckDB table in the project's `.soil` directory (if exists).
3. Use high-bandwidth querying (grep/SQL) to recall this state upon return, ensuring zero re-discovery latency.

## Workflow 3: Pressure Map Analysis
1. Before execution, perform a "depth check" on the project's historical commits and architectural layers.
2. Simulate the impact of changes across all layers (Surface, Engine, Soil) simultaneously.
3. Verify deterministic outcomes in a sandboxed environment (Gemini CLI) before final deployment.
