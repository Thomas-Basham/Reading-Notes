# Class 16

## Reading

### [What is Serverless Computing?](https://www.ibm.com/cloud/learn/serverless)
- Serverless is a cloud computing execution model that 

      Automatically provisions the computing resources required to run application code on demand, or in response to a specific event;
      Automatically scales those resources up or down in response to increased or decreased demand;
      Automatically scales resources to zero when the application stops running. 
- There are most definitely servers in serverless computing
- Functions as a Service (FaaS) is a type of cloud-computing service that allows you to execute code in response to events without the complex infrastructure typically associated with building and launching microservices applications.
- There are several best practices you can follow to make using FaaS easier to deploy and more effective:

      Make each function perform only one action: FaaS functions should be designed to do a single piece of work in response to an event. Make your code scope limited, efficient, and lightweight so functions load and execute quickly.
      Don’t make functions call other functions: The value of FaaS is in the isolation of functions. Too many functions will increase your costs and remove the value of the isolation of your functions.
      Use as few libraries in your functions as possible: Using too many libraries can slow functions down and make them harder to scale.
- Great for stateless/REST 
## Additional Resources

### [venv - Creation of Virtual Environments](https://docs.python.org/3/library/venv.html)

### [Vercel - Get Started](https://vercel.com/docs/get-started)

### [http.server](https://pymotw.com/3/http.server/index.html)

### [Requests](https://docs.python-requests.org/en/latest/)

### [Python & APIs](https://realpython.com/python-api/)
## Videos

### [What is Serverless?](https://www.youtube.com/watch?v=vxJobGtqKVM)

## Bookmark and Review

### [Serverless Functions](https://vercel.com/docs/concepts/functions/serverless-functions)

### [Effective Python Environment](https://realpython.com/effective-python-environment/)