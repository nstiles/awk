# awk - Chapter 1 

emp.data is the file that contains some employee information 

## Examples 

Print out the wages for the employees that have hours.
 
 ```sh
awk '$3 > 0 { print $1, $2 * $3 }' emp.data

Kathy 40
Mark 100
Mary 121
Susie 76.5
```

Print out the employee names that had zero hours
 
 ```sh 
awk '$3 == 0 { print $1 }' emp.data
```

  Beth
  Dan
