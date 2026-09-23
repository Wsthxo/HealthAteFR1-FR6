# HEALTHIATE - FR1 Prototype Specification

## Reference Sources

I will provide:

1. System Architecture reference
2. Figma Prototype reference screenshots

Analyze both references **BEFORE writing any code**.

- **System Architecture** = source of truth for FR1 flow, inputs, and outputs.
- **Figma Prototype** = source of truth for UI design and screen layout.

Do not guess or redesign anything that is already defined in the references.

---

## FR1: Food Component Analysis

### Main Flow

User
→ Upload / Take Food Image
→ AI analyzes the food
→ Display analyzed food components
→ Display nutrition information
→ Display relevant risk / warning information
→ Return to Home

Follow the FR1 input/output shown in the System Architecture.

Do not invent a different process or add unrelated functionality.

---

## UI Requirements

Use the Figma screenshots as the **VISUAL SOURCE OF TRUTH**.

Match the reference as closely as possible:

- Element positions
- Element sizes
- Colors
- Typography
- Cards
- Buttons
- Header
- Bottom navigation
- Spacing
- Screen flow
- Overall visual style

Keep all screens visually consistent with the existing Figma design.

Do not redesign the UI unless necessary for functionality.

---

## Functional Prototype

This must be a **WORKING INTERACTIVE PROTOTYPE**, not static UI.

The user must be able to complete the entire FR1 flow.

### Required functionality

- Functional navigation
- Functional buttons
- Upload food image
- Image preview
- Analyze button
- Loading state
- Simulated AI analysis
- Display food analysis results
- Display nutrition information
- Display relevant food risk / warning information
- Return to Home
- Basic error / empty states

Use realistic mock data to simulate the AI analysis.

No backend, database, or external AI API is required at this stage.

Use React state or localStorage for temporary data if needed.

Do not create fake or non-functional buttons.

---

## Before Coding

1. Inspect the existing project.
2. Check `package.json`.
3. Identify the framework.
4. Inspect the current project structure.
5. Inspect existing components and styles.
6. Reuse existing components and styles where possible.
7. Do not delete or rewrite existing code unnecessarily.

---

## Implementation Rules

- Keep the existing framework.
- Keep the existing project structure.
- Avoid unnecessary dependencies.
- Keep the code simple and maintainable.
- Use mock data only.
- Focus only on FR1.
- Do not implement FR2–FR6.

---

## Testing

After implementation:

1. Run the project.
2. Test the complete FR1 flow from Home to Analysis Result.
3. Test image upload.
4. Test all buttons and navigation.
5. Check responsive mobile layout.
6. Fix any errors.
7. Make sure the prototype is ready for a live demonstration.

---

## Final Report

After completing the implementation, briefly report:

- Files created
- Files modified
- Main components
- FR1 flow implemented
- How to run the project
- Any limitations of the prototype


## FR1 Food Analysis Logic

The system should simulate a real food analysis pipeline:

Food Image
→ Food Detection
→ Food Segmentation
→ Food Classification
→ Portion Estimation
→ Nutrition Calculation
→ Risk Analysis
→ Result

The system should identify individual food components such as:
- Vegetables
- Meat / Protein
- Rice / Carbohydrates
- Fat
- Other food components

For the prototype, use mock detection and nutrition data.
Do NOT implement a real AI model yet.

The result screen should visually show:
- Original food image
- Detected food components
- Food category
- Estimated portion
- Calories
- Protein
- Carbohydrates
- Fat
- Sodium
- Risk / warning level
- Health recommendation

Simulate the analysis process with loading states:
1. Detecting food
2. Separating food components
3. Identifying ingredients
4. Calculating nutrition
5. Analyzing risks
6. Showing results

The prototype should make the user experience feel like a real AI food analysis system.