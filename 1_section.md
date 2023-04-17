
# Welcome to ai starter : Part I

In this tutorial series, we will build a web application that uses OpenAI for text completion. The application will run in the browser and allow users to enter a prompt in a text field and receive a completion from OpenAI in a text area.

## Prepare the project environment
1.  Install virtualenv:
    
	   > `pip install virtualenv` 
    
2.  Create a new directory for your project:
   
	   > `mkdir AI_STARTER` 
    
3.  Create a new virtual environment inside the project directory:

    >  `cd AI_STARTER `  
    >  `virtualenv env`

    
4.  Activate the virtual environment:
    
    On Windows:
    >  `env\Scripts\activate`

    On macOS/Linux:
 
	> `source env/bin/activate`
    
5.  Install Flask:

	> `pip install flask`
	
6. At this point, I recommend using a good code editor. For me, I'm using [Visual Studio Code](https://code.visualstudio.com/) (Good, free, and helpful for deployment)
7. Open Visual Studio Code
8. Open the directory project, at this level your project directory contains only the env directory
![](https://github.com/dalila-taleb/ai_starter_tutorial/blob/main/Capture%20d'%C3%A9cran%202023-03-15%20001241.png?raw=true)

## Create the V1 of your application
1.  Create a new file named main.py in the project directory:

	> main.py


2.  Open main.py and add the following code:
> 	
>     from flask import Flask
>     app = Flask(__name__)
>     
>     @app.route("/")
>     def hello():
>         return "Hello, AI World!"
>     
>     if __name__ == "__main__":
>         app.run(debug=True)

	    

3.  Save the file.

## Run the application : 

From Visual Studio Code :

> F5
> For the first execution, you will get a prompt configuration :
![](https://github.com/dalila-taleb/ai_starter_tutorial/blob/main/Capture%20d'%C3%A9cran%202023-03-15%20001346.png?raw=true)

> Select Flask and click **enter**
> Then, you will be invited to give the file name 
![](https://github.com/dalila-taleb/ai_starter_tutorial/blob/main/Capture%20d'%C3%A9cran%202023-03-15%20001420.png?raw=true)
> Tape : main.py and **enter**

From terminal :
> `python main.py` 
    
You should see output similar to the following:
    
  Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
  
## Finally, see the result:
Launch your browser and tape http://127.0.0.1:5000/ in the URL and enjoy it !

![](https://github.com/dalila-taleb/ai_starter_tutorial/blob/main/Capture%20d'%C3%A9cran%202023-03-15%20001616.png?raw=true)
