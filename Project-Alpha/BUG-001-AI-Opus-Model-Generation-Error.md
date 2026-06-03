# [BUG-001] AI Model Opus 4.7 Fails Document Generation on First Prompt with Configuration ValueError

**Component:** AI Features / Workspace Studio Chat Integration  
**Priority:** High  
**Severity:** High Severity  
**Environment:** STG; MacBook Air M4 (2025); macOS 26.4.1 (ARM); Chrome 147.0.7727.138  
**Reproducibility Rate:** 100% (Isolated to Opus 4.7 model)  

## Preconditions
1. The user is successfully authenticated (Logged in).
2. A project folder named "Business Plan" has been created within the workspace.
3. The AI model selection is explicitly set to "Opus 4.7".

## Steps to Reproduce
1. Open the previously created "Business Plan" project.
2. Click the "AI Chat button" located in the top-right corner of the viewport.
3. Enter the following prompt into the AI chat field and submit: "Write a 2 page business plan for a coffee shop in Manhattan, New York"
4. Wait for the error response, then resubmit the exact same prompt into the AI chat field for a second time.

## Expected Result
On the very first request, the system should correctly communicate with the chosen AI model configuration, process the input parameters, and generate the corresponding text/document output within the workspace studio without errors.

## Actual Result
* **On the first prompt request:** The system fails to generate the document and returns a configuration validation error: `[Error] Writing failed: {'error': ValueError('No draft_id (document_id) found in config'), ...}`. In some instances, the system fails silently and returns no response at all.
* **On the second prompt request:** The system successfully generates the correct textual output.

