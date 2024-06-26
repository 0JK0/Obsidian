#documentation
### Description

A Workout Tracking "app" run from the terminal, it should allow to view, update, and register the date of a routine.

### How?

I'm planing to make it using SQLite and Python i don't want a GUI since apart from the fact i don't feel like learning how to make one, i just feel like is kinda cooler if it is used without a GUI

#### Using experience:

The way the user(me) is going to interact with the "app" should go something along the lines of:

- Ask for options (1.Show all available Routines 2.Show Workout History)

- #### if option 1 is chosen:

- Display routines table

- Chose your routines

- display the table for that specific routine then ask (1.View 2.Use 3.Update)
	
    - **View mode:** shows the table again
    
    - **Use mode:** display 1 by 1 each workout (row), it will display a counter to count sets, after it reaches the amount of sets it will give a resting timer and move to the next workout(row). When it finishes it should display the amount of time taken and save: the routine done, the date and the time it took in another table; Finally show the History table and ask if they want to (1.Quit 2.Go back to menu)
	
	- **Update mode:** Allow to change amount of sets,reps or workouts in said routine then just go to view mode.


- #### if option 2 is chosen:

- Show the History table and ask for (1.Quit 2.Go back to menu)
