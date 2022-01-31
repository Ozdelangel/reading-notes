# Serverless Computing
- Serverless is a cloud execution model that enables a simpler, more cost-effective wau to build and operate could-native applications


## more on that
- Automatically provisions the computing resources required to run application code on demand, ir in response to a specific event
- Automatically scales those resources up or down in response to increased or decreased demand
- Automatically scales resources to zero when the application stops running
- Serverless offloads all management responsibility for backend cloud infrastructure and operations tasks - provisioning, scheduling, scaling, patching and more - to the cloud provider. 
- Makes more time for developers to develop and optimize their front end application code and business logic

## history
- AWS introduced serverless in 2014 with aws lambda
- Faas is actually a subset of serverless


# pros
- They help developers focus more on codr
- Customers pay for execution only
- Serverless is a polyglot environment, enabling developers to code in any language
- Serverless simplifies deployment



# Serverless Functions
With vercel, you can deploy serverless functions, which are pieces of code written with a backend language that take an HTTP request and provide a response 
You can use serverless functions to handle user authentication, form submission, database queries, custom slack commands, and more
## Deploying Serverless Functions
To deploy without any additional configuration, you can put files with extensions matching supported languages and exported function in the `api` directory at your project root
Then push to your connected Git repository using a vercel for git to receive a deployment automatically. 
## Environment Variables 
You can configure environment variables of you serverless functions directly from project settings.
