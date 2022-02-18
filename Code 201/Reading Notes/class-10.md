# Class 10

## From the Duckett JS book

    JavaScript book, Ch. 10, “Error Handling & Debugging”
        pg 449-486

        It's important to know the order of execution of your code/functions so that you can find errors in your code easier

        using the console and console logs will help you find errors by using the method console.log(); along your code where you may have problems

        other onsole methods. these will display differently in the console 

        console.info()  for general infromation 
        console.warn()  for warnings 
        console.error()  for errors 

        try catch and finally is useful if you know your code might fail. three seperate code blocks:

        try {
                <!-- try this code first -->
        } catch (exception){
                <!-- if the try code throws an exception, catch steps in with an alternative set of code. has one param: the error object -->
        } finally {
                <!-- the contents of the finally code block will run either way -->
        }

        If you try to mix a string with a number you will get NaN error
