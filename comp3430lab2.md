# Lab 2

# exercise 1
## screenshots

## board 
<img width="1354" alt="myboard" src="https://user-images.githubusercontent.com/66326548/125123471-533e5700-e0bc-11eb-8943-738fbdeb51e1.png">

## pi 
<img width="1354" alt="mypi" src="https://user-images.githubusercontent.com/66326548/125123492-59ccce80-e0bc-11eb-93c4-ec1c45da8fe2.png">

## state.stp
<img width="1353" alt="mystate" src="https://user-images.githubusercontent.com/66326548/125123560-6e10cb80-e0bc-11eb-997b-52713fd80e49.png">

## description 
The state from previous task to next task is from 1 to 0 or 0 to 1, which means if the previous task state is intterupted, the next task state is on running. 
In board.c, the name gnome-terminal state is 0 and its previous task state is also 0, and its previous task pid is 0 as well, same with the task whose name is stapio with pid 26344. if the previous task pid is 0, its next task state will be 0 as well which means running. 
In pi.c, it starts with state 0, while it is always 0, it will eventually get interrupted and the state will turn to 1.



# exercise 2
## screenshots 

## board
<img width="923" alt="exercise2board" src="https://user-images.githubusercontent.com/66326548/125124006-0e66f000-e0bd-11eb-888f-feb347e8ad8e.png">


## pi
<img width="1007" alt="exercise2pi" src="https://user-images.githubusercontent.com/66326548/125124009-0f981d00-e0bd-11eb-9a85-26c7920c7585.png">


## no -c option
<img width="903" alt="exerciseno-c" src="https://user-images.githubusercontent.com/66326548/125124012-1030b380-e0bd-11eb-8bde-ad31fc429bb1.png">

## description 
schedtimes.stp provides execname, pid, run, sleep, iowait, queued and totall in us. but my script provides execname, pid, state and cpu of each task.
schedtimes.stp keeps track of the task and monitor more information about the task, which gives us more detailed information and it can show us how long does the task take and when does the task will need to wait. 

