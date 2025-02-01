**activity #1**
This script provides an API that calculates the factorial of a given number using FastAPI. It includes an endpoint GET /factorial/{starting_number} that computes the factorial of a given number. If the number is negative, an error is returned. If the input is 0, the response is False. Otherwise, the computed factorial is returned.

- Computes the factorial of a given starting_number.

- Returns an error if the number is negative.

- Returns False if the input number is 0.

- Returns the factorial result otherwise.

**activity #2**
This script provides a simple CRUD-based task management API, allowing users to create, read, update, and delete tasks. It includes endpoints to fetch a task by    ID (GET /tasks/{task_id}), create a task (POST /tasks), update a task (PATCH /tasks/{task_id}), and delete a task (DELETE /tasks/{task_id}). The task data model 
includes a task ID, title, optional description, and completion status.: Fetch a specific task by ID.

**- POST /tasks:**

  - Creates a new task.

  - Requires task_id, task_title, and optional task_desc.

  - Returns an error if task_id already exists.

**- PATCH /tasks/{task_id}: Updates an existing task's title, description, or status.**

**- DELETE /tasks/{task_id}: Deletes a task by ID.**

**activity #3**
This script demonstrates how to interact with external APIs, manipulate data, and reformat responses. It includes endpoints to fetch all posts (GET /posts/), fetch a specific post (GET /posts/?postId={id}), fetch all comments (GET /comments/), fetch comments for a specific post (GET /comments/?postId={id}), format posts by user ID (GET /formatted_posts/{userID}), format comments for a post (GET /formatted_comment/{postID}), and fetch all posts with comments for a user (GET /detailed_post/{userID}).


- **GET /posts/?postId={id}**

  - Fetches a specific post by postId.

- **GET /comments/**

  - Fetches all comments from the external API.

- **GET /comments/?postId={id}**

  - Fetches comments related to a specific post.

- **GET /formatted_posts/{userID}**

  - Returns posts belonging to a given user, formatted for readability.

- **GET /formatted_comment/{postID}**

  - Returns comments related to a specific post, formatted for readability.

- **GET /detailed_post/{userID}**

  - Fetches all posts from a specific user along with their corresponding comments.
**activity #4**
This FastAPI application provides a CRUD-based task management system with API key authentication and versioned endpoints (/apiv1 and /apiv2). APIV1 supports basic task retrieval, while APIV2 enables full CRUD operations, including creating, updating, and deleting tasks.

