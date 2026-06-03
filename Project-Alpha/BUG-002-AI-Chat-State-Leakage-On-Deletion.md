# [BUG-002] Active AI Generation Request Leaks and Continues Processing in Newly Created Chat Session After Deletion

**Component:** AI Features / Chat Session Lifecycle Management  
**Priority:** High  
**Severity:** High Severity  
**Environment:** PROD; MacBook Air M4 (2025); macOS 26.4.1 (ARM); Chrome 147.0.7727.138  
**Reproducibility Rate:** 100%  

## Preconditions
1. The user is successfully authenticated (Logged in).
2. A general document named "BP 3" has been created within the workspace.

## Steps to Reproduce
1. Open the "BP 3" document.
2. Open the AI Chat interface.
3. Select the "Gemini 3.1 Pro" model from the model dropdown selection.
4. Submit a complex text generation prompt to initiate the AI "thinking"/processing state.
5. Create a new chat session.
6. Immediately delete the previous (active) chat session.

## Expected Result
1. The newly created chat session must be completely blank and initialized in an empty state.
2. The active background asynchronous request and the AI generation processing for the deleted chat must be immediately aborted/terminated upon session deletion, preventing data leakage into subsequent sessions.

## Actual Result
Despite deleting the active chat session, the pending background generation request is not terminated. The system leaks the application state, causing the AI to continue processing and automatically stream the response payload directly into the newly created, unrelated chat session.

