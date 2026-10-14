//CORS ---
- Location: AuthController/ProjectController
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: @CrossOrigin(origins = "*")
- Impact: High
- Priority: High
- Proposed solution: Use frontend origin instead of all origins
- Verification: Verified
- Implementation notes:

//register ---
- Location: AuthController
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: No user check
- Impact: Medium
- Priority: High
- Proposed solution: First check for user existence before adding
- Verification: Verified
- Implementation notes:

//register ---
- Location: AuthController
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 25
- Impact: High
- Priority: High
- Proposed solution: Hide password on JSON return
- Verification: Verified
- Implementation notes:

//login ------
- Location: AuthController
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 32
- Impact: Medium
- Priority: Medium
- Proposed solution: Pass in an exception in the orElseThrow
- Verification: Verified
- Implementation notes:

//login  ---------
- Location: AuthController
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 33 - 34
- Impact: High
- Priority: High
- Proposed solution: Have a condition that has return statement end the method when the passwords don't match
- Verification: Verified
- Implementation notes:

//project ----
- Location: ProjectController
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 32
- Impact: Medium
- Priority: Medium
- Proposed solution: Use .orElseThrow() with the appropriate exception include 
- Verification: Verified
- Implementation notes:

//Task -----
- Location: TaskService
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 43
- Impact: HIgh
- Priority: High
- Proposed solution: Use derived query instead to prevent SQL injection
- Verification:Verified
- Implementation notes:


//frontend  -------
- Locations: TaskBoard.tsx
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 12
- Impact: HIgh
- Priority: High
- Proposed solution: Pass the projectId for a re run when projectId changes
- Verification: Verified
- Implementation notes:

//frontend  
- Locations: TaskBoard.tsx
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 12
- Impact: HIgh
- Priority: High
- Proposed solution: Pass the projectId for a re run when projectId changes
- Verification: Not Verified
- Implementation notes:

//frontend ----
- Locations: TaskBoard.tsx
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 17
- Impact: HIgh
- Priority: High
- Proposed solution: Use the spread operator
- Verification: Verified
- Implementation notes:

//frontend ----- 
- Locations: TaskItem.tsx
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 15
- Impact: HIgh
- Priority: High
- Proposed solution: replace {task.name} with {task.title}
- Verification: Verified
- Implementation notes:

//properties  
- Locations: 
- Status: observed | suspected | confirmed | fixed | deferred
- Evidence: line 15
- Impact: HIgh
- Priority: High
- Proposed solution: replace {task.name} with {task.title}
- Verification:
- Implementation notes:

