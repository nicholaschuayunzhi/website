### `for` Statements

You can **use a `for` statement, together with the `range()` function, to repeat a code block a pre-determined number of times.** 

Format:
```
for variable_used_as_index in range(number_of_times_to_repeat) :
    statements_to_repeat
```

<tip-box>

:package: the code below use a `for` loop to iterate three times. Note how the variable `i` is used as an indexing variable and how `i in range(3)` causes `i` to take values `0, 1, 2` over the three iterations. 

<table>
<tr>
  <td>
  
```python
for i in range(3):
    print(i, 'Knock knock, Penny!')
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```
0 Knock knock, Penny!
1 Knock knock, Penny!
2 Knock knock, Penny!
```
  </td>
</tr>
</table>

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/penny-thrice?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

:bulb: Note how the above example uses `print()` with two parameters, one an integer and one a string. The `print()` method can take multiple parameters and the parameters can be of different types. Note that the ==output will have a space between each parameter==. 

<table>
<tr>
  <td>
  
```python
print('ABC', 3, 4.50)
print('ABC' + str(3) + str(4.50))
print('ABC' + ' ' + str(3) + ' ' + str(4.50))
```
  </td>
  <td>&nbsp;→&nbsp;</td>
  <td>
  
```

ABC 3 4.50
ABC34.50
ABC 3 4.50
```
  </td>
</tr>
</table>


</tip-box>

<panel type="danger" header=":muscle: Exercise: Multiplication Table" expanded no-close>
  <include src="e-multiplicationTable.md" />
</panel><p/>

**You can use `break` and `continue` in `for` loops as well**, with similar effects as in `while` loops.

<tip-box> 

:package: The code below totals the numbers entered by the user. It uses `range(5)` to limit the number of entries to 5. It uses a `break` to exit the loop if user hits <kbd>Enter</kbd> without entering a value. It uses a `continue` statement to skip negative numbers entered by the user.


```python
total = 0
for n in range (5):
  number_as_string = input('Enter a number (press enter to exit):')
  
  # exit if user input is empty
  if number_as_string == '':
    print('Exiting as per user request...')
    break
    
  # convert the input into an integer
  number_as_int = int(number_as_string)
  
  # skip if the number is negative
  if number_as_int < 0 :
    print('Negative number, skipped')
    continue 
    
  # update the total and print the running total
  total = total + number_as_int
  print('Running total:' + str(total))

print('Grand total of non-negative numbers:', str(total))
```

<panel type="seamless" header="%%:computer: Try your own%%">

<iframe height="400px" width="100%" src="https://repl.it/@pythonbasics/addup-positive?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

</panel><p/>

</tip-box>