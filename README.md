# MarketplaceCoursera
Creating a marketplace application for online course .
1. Authentication Page:   - Create a simple login field.
   - The user must enter a username to log in.
   - It is not necessary to implement true authentication; a static username verification is sufficient.

2. Viewing Courses:
   - Display a list of courses.
   - Each course must have: id, image, title, description, categories, author.
   - For each category, the first 4 courses must be displayed.

3. Upload New Course:   - Only authenticated users can upload new courses.
   - Provide a form to enter course details (title, description, image, categories).

4. Detail and Edit Course:
   - Upon clicking on a course, open a modal to view its details.
   - If the user is authenticated, allow editing of the course in the same modal.
   - Implement a toggle to switch between viewing and editing.

5. Course Deletion:
   - Add option to delete a course (for authenticated users only).

Data Structure:
- `username`: string
- `courses`: Array of objects with { id, srcImg, title, description, categories, author where author corresponds to the logged-in username }

JavaScript functions:
- `createCourse({ title, description, srcImage, categories })`: To add a new course.
- `editCourse({ id, title, description, author, srcImage, categories })`: To edit an existing course.
- `deleteCourse(id)`: To delete a course
