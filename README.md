# arweave-journal-summary  
This python program takes in the journal data which includes arweave log information and creates a two line  
summary for each group of storage module displays that occur in the log, thus reducing the amount of data  
output but giving a good summary of activity.  The full log can also still be viewed with the Linux command  
journalctl -f.  There is no need to modify the contents of this program but it will need to be modified when  
the storage module numbers increase over time.  It currently ends with module 38 and can be changed as needed  
by modifying line max_partition = 38. The summation line that includes full weave is a sum of the values from  
all storage module lines and Sample output is below:  

2023-05-23 21:33:15.922622 - Total avg: 408.73 MiB/s,  1634.92 h/s; current: 263.44 MiB/s, 1053.77 h/s; VDF: 1.01 s.  
2023-05-23 21:33:25.922353 - Total avg: 408.73 MiB/s, current: 263.44 MiB/s, optimum: 2391.35 MiB/s, full weave: 4782.69 MiB/s  
2023-05-23 21:33:25.922398 - Total avg: 408.73 MiB/s,  1634.93 h/s; current: 414.04 MiB/s, 1656.16 h/s; VDF: 0.91 s.  
2023-05-23 21:33:35.922528 - Total avg: 408.73 MiB/s, current: 414.04 MiB/s, optimum: 2146.50 MiB/s, full weave: 4292.99 MiB/s  
2023-05-23 21:33:35.922582 - Total avg: 408.69 MiB/s,  1634.75 h/s; current: 335.92 MiB/s, 1343.69 h/s; VDF: 0.91 s.  
2023-05-23 21:33:45.922589 - Total avg: 408.69 MiB/s, current: 335.92 MiB/s, optimum: 2141.77 MiB/s, full weave: 4283.59 MiB/s  
2023-05-23 21:33:45.922643 - Total avg: 408.64 MiB/s,  1634.56 h/s; current: 333.67 MiB/s, 1334.69 h/s; VDF: 0.91 s.  
2023-05-23 21:33:55.922632 - Total avg: 408.64 MiB/s, current: 333.67 MiB/s, optimum: 2142.86 MiB/s, full weave: 4285.72 MiB/s  
