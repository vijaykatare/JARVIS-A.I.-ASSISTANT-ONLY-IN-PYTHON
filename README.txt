WELLCOME SCREEN

	MINOR PROJECT
	JARVIS A.I. DESKTOP ASSISTANT #PYTHON

Have you ever wondered how cool it would be to have your own A.I. assistant ? Imagine how easier it would be to sendemail without typing a single word, doing Wikipedia search without opening web browsers , and performing many other daily tasks like playing music with the help of a single voice command. 

PROJECT MEMBERS- Mr. Vijay Katare , Mr. Subrat jain , Mr. Nikhil Panjwani , Mr. Harsh Rajpoot , Mr. Chali Prasad Lodhi 
   

	WHAT CAN THIS A.I. ASSISTANT DO FOR OUS ?

•	It can send emails on your behalf.
•	It can play music for you.
•	It can do Wikipedia searches for you.
•	It is capable of opning your code editor or IDE with a single voice commands.
ENOUGH TALKS !
LET’S  Start building our own J.A.R.V.I.S.

	STARTING V.S. CODE

We are going to use the V.S. code IDE for this project.  Start a new project and make a file called Jarvis.py



	DEFINING SPEAK FUNCTION

The first and foremost thing for an A.I. assistant is that it should be able to speak. To make our on J.A.R.V.I.S. talk , we will make a function called speak() . This function will take audio as an argument, and then it will pronounce it. 



Def speak(audio):
          pass    #we will write the conditions later.
Now. The next thing we need is audio. We must supply audio so that we can pronounce it using the speak() function we made.
WE ARE GOING TO INSTALL  Pyttsx3

	What is pyttsx3 ?

•	A python  library that will have us to convert text to speech. In short, it is a text – to – speech library.
•	It works offline, and it is an compatible with python 2 as well as python 3.



	INSTALLATION:

Install pyttsx3 by typing the below command in the terminal:


pip  install pyttsx3
           after installing pyttsx3 , import this module into our program.
	USAGE:

Import pyttsx3
engine = pyttsx3.init ( ‘sapi5’ ) 
voice = engine.getProperty( ‘voices’ ) #getting details of current voice
engine.setProperty( ‘voice’ , voice[0] . id)
	What is sapi5 ?

•	Microsoft developed speech API.
•	Help in synthesis recognition of voice.


	What is voiceld ?

•	voice id help us to select different voices.
•	voice[0].id = male voice
•	voice[1].id = female voice


	Writing Our speak() Function :	

We made a function called speak() at the starting of this project. Now, we will write our speak() function to convert our text to speech.

Def speak(audio):
engine.say(audio)
engine.runAndwait()                     #without this command, speech will not be audible to us.





	Creating our main() function:

we will create a main() function, ans inside this main() function, we will call our speak function.




	Code:


if __name__==”__main__” :

speak(“Adina ”)

Whatever you will write inside the speak() function will be converted Into speech. Congratulations! With this, our J.A.R.V.I.S . has its own voice, it is ready to speak.


	Difining wish me function  :


Now we will make a wishme() function that will make our J.A.R.V.I.S. wish or great the user according to the time of computer or pc.
To provide current or live time to A.I. we need to import a module called datetime. Import a module in our program by: 
