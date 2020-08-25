# What I found out

We gitignore the functions directory or wherever we write our functions because netlify can't do anything with that

We can mitigate CORS errors with the appropriate headers in our server response by adding a headers property to our returned object

In production, if you want to access the API, you would need to use the endpoint of the function which is generally /.netlify/functions/{function_name} but in development you can use localhost. use env variables for easy swapping

We can specify environment variables during our deployment step but these variable names must match the ones used in our code.
