# Frockly: Advanced Developer Enhancements

Advanced enhancements for [Frockly](https://github.com/RyuU12358/Frockly) by [@montesito](https://github.com/montesito), contributing to the original work by [@RyuU12358](https://github.com/RyuU12358).

This suite introduces a **modern, minimalist UX** designed to streamline professional formula development. By simulating high-fidelity Excel behaviors and adding advanced capabilities—including Excel-native exporting and intelligent LET/LAMBDA creation with integrated testing—these updates provide a robust, intuitive environment for complex formula engineering.

All features have been successfully implemented and validated on **macOS** (only).

---

## 🚀 Key Enhancements

### 1. Modernized User Interface (UI/UX)
Revised the application architecture to maximize workspace efficiency while maintaining the corporate brand identity.

*   **Header Reorganization**: Optimized vertical space by reducing component dimensions and font sizes.
*   **Integrated Search**: Relocated the search bar to the "Functions" tab, enabling real-time filtering of formula definitions.
*   **Intuitive Tooltips**: Restructured formula metadata displays for improved readability during hover interactions.
*   **Enhanced Discovery**: Strategic repositioning of the "From Formula" import feature for better workflow integration.
*   **Flexible Layouts**: Implemented draggable dividers allowing users to manually resize the main panels (Grid vs. Editor) to suit their current task.

![UI Overview](assets/UI_General_Overview.gif)


---

### 2. High-Fidelity Data Grid
The cell grid has been overhauled to provide an experience closer to professional spreadsheet software.

*   **Keyboard Navigation**: Full support for arrow key navigation and selection cycles.
*   **Intelligent Data Entry**: Data-type aware formatting (right-aligned numbers, left-aligned text) allows for immediate in-app data validation without external workbooks.
*   **Excel-Standard Behavior**: The `Enter` key now natively advances the selection to the subsequent row.
*   **Dynamic Sizing**: Support for manual row height and column width adjustments.
*   **Performance Optimization**: Significant reduction in latency for grid updates and input rendering.
*   **Formatted Formula View**: The formula bar now preserves and displays syntax-highlighted and indented formulas for better auditing.

![Grid Interactivity](assets/Grid_Interactivity_and_Performance.gif)

---

### 3. Integrated Logic Editor
Improvements to the block-based editing environment to facilitate rapid formula construction.

*   **Horizontal Layout Transition**: Converted the central vertical controls (Basic, Names, History) into a streamlined horizontal toolbar at the top of the workspace.
*   **Workspace Optimization**: Reduced grid density and adjusted color contrast to minimize visual fatigue during long development sessions.
*   **Contextual Templates**: Upon selecting a formula, a dynamic panel demonstrates usage examples. Users can immediately insert pre-configured block structures.
*   **Smart Selection Magnifier**: Enhanced Cell and Range blocks with a "Magnifier" tool for direct grid-based selection, reducing manual coordinate entry.
*   **Active Block Tracking**: The UI now dynamically updates to show the formula representation of the *currently selected* block, rather than defaulting to the first block in the workspace.
*   **Validation-Aware Insertion**: The "Insert" button now performs circular reference checks before pushing formulas from the editor to the grid.

![Block Editor Workflow](assets/Block_Editor_Workflow.gif)

---

### 4. Advanced Formula Support
Deep architectural fixes for complex logic handling.

#### **LET Function**
*   Refined block generation logic for variable assignment.
*   Increased robustness in the de-blockification engine to handle complex nested scopes.

#### **LAMBDA Function**
*   **Advanced In-Place Testing**: A new "Intelligent Test" mode identifies required parameters and opens a dedicated modal for selection.
*   **Automated Parameter Injection**: Parameters are automatically formatted and passed to the LAMBDA function for testing within the app environment.

![Advanced Formulas](assets/Advanced_Formulas_LET_LAMBDA.gif)

---

### 5. Seamless Interoperability
*   **Professional Exporting**: Added "Export as Excel" functionality that generates native `.XLSX` files.
*   **Locale Independence**: Automatically handles system-specific formula separators (e.g., `,` vs `;`) ensuring the generated files evaluate correctly in any regional Excel installation.

![Excel Export](assets/Excel_Export_Interoperability.gif)

---

## 📁 Repository Structure
*   `/assets`: Contains detailed walkthrough GIFs for each of the features mentioned above.
*   `/src`: Core application logic and block definitions.
*   `/public`: Static assets and branding.

---

> 一矢(いっぴゃ)は折(お)れ易(やす)く、十矢(じゅうや)の束(たば)は折(お)れぬ

Developed with precision for the Frockly community.
