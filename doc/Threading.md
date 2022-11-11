First, I create a function called initial() within Stage.java,
Where the ai(isBot==True) of the actors are split into their own thread.
This is done by going through the list of actors,
and if the actor is a bot, send it to a thread and run that thread.
Finally, as the bots were running too fast, I added a thread.sleep() to
pause the thread, keeping it in time with the main thread.

All of this is contained in Stage.java in lines 37 to 69.



Finally, I created a call to the aforementioned function in
the building of the stage.
Located in Main.java at line 111.