# text-expander
The Git repository contains a React application that implements a text expander component. The component allows users to display and expand or collapse text content based on the specified configuration.

The App component serves as the entry point of the application. It renders multiple instances of the TextExpander component with different configurations and content. Each TextExpander component represents a block of text that can be expanded or collapsed.

The TextExpander component accepts the following props:

- `collapsedNumWords` (optional): Specifies the number of words to display when the text is collapsed. Default value is 10.
- `expandButtonText` (optional): Specifies the text for the expand button. Default value is "Show more".
- `collapseButtonText` (optional): Specifies the text for the collapse button. Default value is "Show less".
- `buttonColor` (optional): Specifies the color of the expand/collapse button. Default value is "#1f09cd".
- `expanded` (optional): Specifies whether the text should be initially expanded or collapsed. Default value is `false`.
- `className` (optional): Specifies an additional CSS class to be applied to the component.
- `children`: The text content to be displayed and expanded/collapsed.

The TextExpander component uses the useState hook to manage the state of `isExpanded`, which determines whether the text is currently expanded or collapsed. The `displayText` variable is computed based on the current state, either displaying the full text or a truncated version.

When the expand/collapse button is clicked, the `isExpanded` state is toggled using the `setIsExpanded` function. This triggers a re-render and updates the displayed text and button text accordingly.

The application showcases the usage of the TextExpander component by rendering multiple instances with different configurations and content. Users can interact with the expand/collapse buttons to control the visibility of the text.

The Git repository includes the necessary code files, including the App component, the TextExpander component, and a CSS file (`styles.css`) for styling the application. Developers can explore the code and styles to understand how to implement a text expander functionality in a React application and customize its appearance and behavior.

Overall, the application provides a convenient and reusable solution for displaying expandable/collapsible text content, allowing users to control the amount of text displayed at once.
