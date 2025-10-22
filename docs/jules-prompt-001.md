# Prompt: Jules – Universal AI UI Library (Deno-Driven)

## Objective
Develop a **universal AI-driven UI Library** as the **single source of truth** for all graphical interfaces (Electron, Web, API) across projects.  
The system must be **accessible**, **composable**, and **AI-readable**, built with **React**, **Tailwind CSS**, **React Aria**, **Storybook**, and **Deno**.  
This library will form a reusable foundation for every future AI or human development task in UI/UX.

***

## References and Learning Sources
- **Untitled UI React Library**  
  Example: https://www.untitledui.com/react/components  
  Learn its component architecture, prop conventions, and layout patterns to inform the base library’s design hierarchy.
- **Deno WebUI**  
  Reference: https://deepwiki.com/webui-dev/deno-webui and https://deepwiki.com/denoland/deno  
  Learn how Deno handles rendering, imports, bundling, testing, and native module execution.
- **Storybook Docs**  
  Reference: https://storybook.js.org/docs  
  Use for visual regression testing, component documentation, and AI-extractable metadata generation.

***

## Jules Task Lifecycle Alignment
- **Phase 1 – Plan Generation:** Analyze examples (UntitledUI structure and Deno WebUI sample repos). Generate a complete build plan covering architecture, dependencies, build flow, CI validation, and folder structure.  
- **Phase 2 – Plan Review:** Await prompt approval before execution.  
- **Phase 3 – Execution:** Implement iteratively, confirming every stage (component creation, Deno integration, documentation) through read verification and Storybook testing.

***

## Technical Stack & Constraints
- **Runtime:** Deno (no Node dependency required)  
- **Languages:** Prefer **pure JavaScript with JSDoc typing** or Deno’s native TypeScript support (decide after analysis for maintainability)  
- **Styling:** Tailwind CSS integrated through Deno-compatible bundling  
- **Accessibility:** Implement React Aria for compliant interactive components  
- **Docs & Testing:** Use Storybook + Deno test integrations (rather than Jest)  
- **Lint/Format:** Rely on Deno’s built-in `lint`, `fmt`, and `check` instead of ESLint/Prettier

***

## Deliverables

1. **UI Component Library**
   - Accessible primitives: Button, Input, Menu, Modal, Toast, Card, Tabs  
   - Complex patterns: Navbar, Dashboard Layout, AuthForm, Grid Layouts  
   - Layout definitions compatible across Web, Electron, and Deno-based renderers  

2. **Documentation**
   - Auto-generate Storybook stories with accessible markup and interaction tests  
   - Include markdown and JSON metadata for AI tool parsing  
   - Provide developer guides (setup, design tokens, conventions) in `/docs/`

3. **Deno Integration**
   - Create `deno.json` for imports and task automation  
   - Demonstrate module usage via Deno WebUI demo  
   - Export modules in a Deno-compatible ESM structure

4. **Architecture Structure**
   ```
   /packages/ui/
     /components/
     /layouts/
     /patterns/
     /tokens/
     /hooks/
   /storybook/
   /docs/
   /deno.json
   ```

5. **Testing and Validation**
   - Use Storybook interaction tests  
   - Run `deno test` for logic validation  
   - Ensure all artifacts pass `deno check` and render correctly via Deno WebUI

***

## Example Commands
```bash
# Setup project
deno task setup

# Run storybook
deno task storybook

# Test components
deno test --import-map=deno.json
```

***

## Execution Steps for Jules
1. Analyze linked references (UntitledUI and Deno WebUI) to map component taxonomy and rendering pipeline.  
2. Generate complete project scaffolding and configuration (`deno.json`, folder structure, basic Storybook setup).  
3. Implement foundational UI tokens and primitives.  
4. Create Storybook stories and accessible documentation.  
5. Validate render compatibility in Deno + Electron + Web environments.  
6. Summarize architecture and readiness checklist.

***

## Output Expectations
- A **validated base project structure** with documentation and first components.  
- **Learning integration** from UntitledUI and Deno WebUI design patterns.  
- An automatically **AI-readable metadata schema** for all components and layouts.  
- A **final summary file** outlining architectural choices, Storybook setup steps, and usage examples.

***
