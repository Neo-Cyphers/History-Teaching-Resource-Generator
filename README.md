# History Teaching Resource Generator Documentation

## What Does It Do?
The **History Teaching Resource Generator** is a web-based tool designed to assist educators and students in creating tailored teaching resources for history topics. It leverages the OpenRouter API to generate educational content based on user inputs, such as resource type, grade level, and historical events. Key features include:

- **Resource Types**: Generates five types of content:
  - 100-word summary
  - Lesson plan
  - Study guide
  - Quiz
  - Compare & contrast (requires two historical events)
- **Customization**: Users specify a grade level and one or two historical events, depending on the resource type.
- **History Tracking**: Saves previously generated resources in the browser’s local storage for easy access.
- **Output Details**: Displays the generated content along with generation time, token usage, and estimated tokens remaining.
- **Download Option**: Allows users to save resources as text files.

## Workflow: How It Works
1. **Input Selection**:
   - The user selects a resource type from a dropdown menu.
   - Based on the selection, the form dynamically updates to request either one or two historical events.
2. **Input Validation**:
   - Ensures the grade level is a valid number.
   - Checks that all required event fields are filled.
3. **Prompt Construction**:
   - Uses predefined templates to create a prompt based on the resource type, grade, and event(s).
4. **API Request**:
   - Sends the prompt to the OpenRouter API for content generation.
5. **Response Handling**:
   - Displays the generated content in a text area.
   - Shows generation time, tokens used, and estimated remaining tokens.
6. **History Management**:
   - Saves the resource details to local storage.
   - Updates the history list for quick access to past resources.
7. **Download Option**:
   - Provides a button to download the current output as a text file.

## Tools and Technologies Used
- **Frontend**:
  - **HTML**: Structures the webpage.
  - **CSS**: Provides styling with a modern, responsive design and animations.
  - **JavaScript**: Manages dynamic updates, API calls, input validation, and local storage.
- **Backend**:
  - **OpenRouter API**: Powers content generation based on user inputs.
- **Storage**: Uses browser local storage to maintain a history of generated resources.
- **Fonts**: Incorporates Google Fonts (Roboto) for a clean, professional look.

## Advantages
- **Ease of Use**: Features an intuitive interface, requiring no technical skills to operate.
- **Flexibility**: Supports multiple resource types and grade levels for customized content.
- **Reusability**: The history feature lets users revisit past resources, saving time.
- **Transparency**: Shows generation time and token usage for each request.
- **Portability**: Resources can be downloaded as text files for offline use or sharing.

## Limitations
- **API Reliance**: Depends on the OpenRouter API’s availability and performance, which could disrupt functionality if the API is down.
- **Token Tracking**: Estimates remaining tokens based on a hypothetical limit (e.g., 10,000), not actual API data, reducing accuracy.
- **Local Storage**: History is stored client-side, limiting capacity and making it unsuitable for multi-user or large-scale use.
- **No Authentication**: Lacks user management, restricting it to single-user scenarios.
- **Basic Error Handling**: Could benefit from more robust error feedback and recovery options.

## How to Use It
1. **Select Resource Type**: Choose from the dropdown (e.g., "Lesson plan").
2. **Input Grade Level**: Enter a numeric grade (e.g., "8").
3. **Add Historical Event(s)**:
   - One event for most types (e.g., "World War II").
   - Two events for "compare & contrast" (e.g., "World War I" and "World War II").
4. **Generate**: Click "Generate Resource" to create the content.
5. **Review**: View the output, stats, and download or revisit past resources as needed.

**Important**: To use this tool, you must download the `History Teaching Resource Generator.html` file located in the `folder1` directory within this repository. Click the link below to automatically download the file. Follow these steps after downloading:
- **Step 1**: Locate the downloaded `History Teaching Resource Generator.html` file on your computer.
- **Step 2**: Double-click the file to open it in your web browser and run it on your local server.
- **Note**: Ensure you have an internet connection to access the OpenRouter API. Replace `'your_api_key_here'` in the code with your actual OpenRouter API key to enable generation functionality.

[Download History Teaching Resource Generator.html](folder1/TEST2.html)

## Additional Considerations
- **Potential Improvements**:
  - Integrate actual token limits from the OpenRouter API.
  - Add user authentication for multi-user support.
  - Expand customization options (e.g., content length, focus areas).
  - Use a server-side database instead of local storage for history.
- **Use Cases**: Ideal for individual educators or students needing quick, tailored history resources, but less suited for collaborative or institutional settings without upgrades.

This tool streamlines the creation of history teaching materials, balancing simplicity with functionality, though its reliance on external services and single-user design are key constraints to consider.
