# A3

## Compile and run

make

./comp3430A3 1 5000 tasks.txt

if you want to recompile, please make clean, and then make, ./comp3439A3 (number of CPUs) (time period) (file.txt)

## Report and analysis

### Question 1

* According to what I have learnt, I expect that the response time and turnaround time should reeduce when we add more CPUs such as 4 CPUs to 8 CPUs. When we change time period from 4000 to 7000, the turnaround time and turnaround time should not change much, because we have random I/O in it and all tasks have chance to run I/O.

### Question 2

* By looking at the table, the turnaround time and response time reduces when we increase the number of CPUs, but when we change the time period only, the turnaround time and response time seem that not change much. So the turnaround time and response time is more effected by the number of CPUs.

## Problems with my program

* The response is clearly not correct, but i have written a method in my code that prints each task's response time when their first time to run, it shows that the order is correct, the first task runs that has a smaller reponse time than the second task that runs. However, sometimes my response time is even smaller than its arrival time or  much bigger than complete time. I also write print method to test that which clock_gettime() run first and after, it also shows that for each task, it gets my arrival time first and then it gets my response time and finally it gets my complete time. I have write comments in my code to explain each step of implementing MLFQ policy. 


#### MLFQ

| Type | CPUs | Time period | Average Turnaround Time | Average Response Time |
| ---- | ---- | ----------- | ----------------------- | --------------------- |
| 0    | 1    | 4000        | 5699                    | 891998                |
| 1    | 1    | 4000        | 3969                    | 713496                |
| 2    | 1    | 4000        | 824                     | 457685                |
| 3    | 1    | 4000        | 1680                    | 627429                |
|      |      |             |                         |                       |
| 0    | 2    | 4000        | 3521                    | 764729                |
| 1    | 2    | 4000        | 1827                    | 644470                |
| 2    | 2    | 4000        | 2026                    | 546520                |
| 3    | 2    | 4000        | 958                     | 635943                |
|      |      |             |                         |                       |
| 0    | 4    | 4000        | 3329                    | 771013                |
| 1    | 4    | 4000        | 1895                    | 593816                |
| 2    | 4    | 4000        | 1579                    | 377880                |
| 3    | 4    | 4000        | 876                     | 648762                |
|      |      |             |                         |                       |
| 0    | 8    | 4000        | 3032                    | 875560                |
| 1    | 8    | 4000        | 1827                    | 672517                |
| 2    | 8    | 4000        | 814                     | 499433                |
| 3    | 8    | 4000        | 1049                    | 498301                |
| Type | CPUs | Time period | Average Turnaround Time | Average Response Time |
| ---- | ---- | ----------- | ----------------------- | --------------------- |
| 0    | 1    | 5000        | 7151                    | 837976                |
| 1    | 1    | 5000        | 4139                    | 602934                |
| 2    | 1    | 5000        | 1229                    | 369040                |
| 3    | 1    | 5000        | 2215                    | 648541                |
|      |      |             |                         |                       |
| 0    | 2    | 5000        | 5472                    | 890953                |
| 1    | 2    | 5000        | 3437                    | 697952                |
| 2    | 2    | 5000        | 1560                    | 501155                |
| 3    | 2    | 5000        | 1299                    | 627552                |
|      |      |             |                         |                       |
| 0    | 4    | 5000        | 3245                    | 849823                |
| 1    | 4    | 5000        | 1813                    | 722464                |
| 2    | 4    | 5000        | 1482                    | 450345                |
| 3    | 4    | 5000        | 1568                    | 549512                |
|      |      |             |                         |                       |
| 0    | 8    | 5000        | 2829                    | 882083                |
| 1    | 8    | 5000        | 1807                    | 644270                |
| 2    | 8    | 5000        | 707                     | 547718                |
| 3    | 8    | 5000        | 1640                    | 588048                |
| Type | CPUs | Time period | Average Turnaround Time | Average Response Time |
| ---- | ---- | ----------- | ----------------------- | --------------------- |
| 0    | 1    | 6000        | 5551                    | 896089                |
| 1    | 1    | 6000        | 3262                    | 700993                |
| 2    | 1    | 6000        | 1731                    | 135653                |
| 3    | 1    | 6000        | 1272                    | 572642                |
|      |      |             |                         |                       |
| 0    | 2    | 6000        | 5026                    | 864536                |
| 1    | 2    | 6000        | 3750                    | 660289                |
| 2    | 2    | 6000        | 820                     | 841175                |
| 3    | 2    | 6000        | 891                     | 693244                |
|      |      |             |                         |                       |
| 0    | 4    | 6000        | 3324                    | 757417                |
| 1    | 4    | 6000        | 1870                    | 580950                |
| 2    | 4    | 6000        | 1164                    | 522822                |
| 3    | 4    | 6000        | 1168                    | 649705                |
|      |      |             |                         |                       |
| 0    | 8    | 6000        | 3039                    | 860905                |
| 1    | 8    | 6000        | 2050                    | 658135                |
| 2    | 8    | 6000        | 1228                    | 433055                |
| 3    | 8    | 6000        | 907                     | 445954                |
| Type | CPUs | Time period | Average Turnaround Time | Average Response Time |
| ---- | ---- | ----------- | ----------------------- | --------------------- |
| 0    | 1    | 7000        | 5330                    | 854654                |
| 1    | 1    | 7000        | 3100                    | 658391                |
| 2    | 1    | 7000        | 608                     | 475194                |
| 3    | 1    | 7000        | 1237                    | 466541                |
|      |      |             |                         |                       |
| 0    | 2    | 7000        | 4904                    | 884764                |
| 1    | 2    | 7000        | 2985                    | 700958                |
| 2    | 2    | 7000        | 932                     | 509775                |
| 3    | 2    | 7000        | 1126                    | 413969                |
|      |      |             |                         |                       |
| 0    | 4    | 7000        | 3841                    | 678967                |
| 1    | 4    | 7000        | 2715                    | 511684                |
| 2    | 4    | 7000        | 1052                    | 720459                |
| 3    | 4    | 7000        | 1507                    | 677340                |
|      |      |             |                         |                       |
| 0    | 8    | 7000        | 3059                    | 871416                |
| 1    | 8    | 7000        | 1752                    | 660596                |
| 2    | 8    | 7000        | 809                     | 553659                |
| 3    | 8    | 7000        | 1345                    | 535389                |

