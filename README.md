# PDF Annotation Tool

## Project Overview

This Vue.js application allows users to drag and drop annotation elements onto PDF pages. Users can place annotations like signatures and stamps on specific locations within PDF pages, and the application will generate a JSON representation of these annotations.

## Functional Requirements

1. Drag and Drop Functionality

   - Users should be able to drag annotation elements from the left sidebar.
   - Annotations should be droppable onto any of the PDF page elements on the right side.
   - The drag operation should visually represent the annotation being moved.

2. Annotation Placement

   - Annotations should snap to the nearest logical position on the PDF page.
   - Multiple annotations should be allowed on a single page.
   - Annotations should remain within the boundaries of the PDF page.

3. Annotation Types

   - Support at least two types of annotations: 'signature' and 'meterai' (stamp).
   - Each annotation type should have a distinct visual representation (by colors)

4. Performance

   - Ensure smooth dragging and dropping, even with multiple annotations and pages.

5. Error Handling
   - Gracefully handle scenarios like invalid drops or out-of-bounds placements.

## Technical Considerations

- Use Vue.js 3 with Composition API.
- Implement drag and drop using native HTML5 API(Recommended) or a Vue-compatible library.
- Use reactive state management for real-time JSON updates.

## Future Enhancements (Nice to have)

- Ability to resize annotations.
- Zoom in/out functionality for PDF pages.
- Support for actual PDF rendering instead of placeholders.
- User authentication and saving annotations to a backend.

## Interview Rules and Guidelines

1. Time Limit:

   - The interview challenge has a duration of 40 minutes.

2. Screen Sharing:

   - Candidates must share their screen throughout the interview process.

3. Resource Usage:

   - Candidates are allowed to browse the internet for solutions and references.
   - Use of online resources should be mentioned to the interviewer.

4. Interaction with Interviewer:

   - Candidates are encouraged to ask questions to the interviewer for clarification.
   - The interviewer may provide hints or guidance if needed.

5. Focus:

   - Priority should be given to implementing core functionalities.
   - Code quality and organization are important, but a working solution takes precedence.

6. Completion:
   - Full completion of all requirements is not mandatory within the time limit.
   - Candidates should explain their thought process and any planned next steps.
