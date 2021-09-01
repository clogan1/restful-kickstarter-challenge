
1. Displays all of the projects
- HTTP Verb & URL: GET '/projects'
- Controller: projects#index
- CRUD: Read
- AR Method: Project.all

2. Displays information about one project
- HTTP Verb & URL: GET '/projects/:id'
- Controller: projects#show
- CRUD: Read
- AR Method: Project.find(params[:id])

3. Creates a new project based on given parameters
- HTTP Verb & URL: POST '/projects'
- Controller: projects#create
- CRUD: Create
- AR Method: Project.create(project_params)

4. Updates an existing project with given parameters
- HTTP Verb & URL: PATCH '/projects/:id'
- Controller: projects#update
- CRUD: Update
- AR Method: Project.find(params[:id]) => Project.update(project_params)

5. Deletes an existing project
- HTTP Verb & URL: DELETE '/projects/:id'
- Controller: projects#destroy
- CRUD: Delete
- AR Method: Project.find(params[:id]) => Project.destroy

