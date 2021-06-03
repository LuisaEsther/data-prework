# Perwork review

Hi Luisa 🙋🏻‍♀️!! I am writing to give you some feedback on your prework! 🚀

### 1. Snail-and-Well

- What happened with the last two exercises??? Only, as a detail, in python yoy have the `mean` and `stdev` functions that give us the mean and standard deviation of a given list of numbers. We only need to import `statistics` library. Here is an example in case you find it usefull:
    ```python
    import statistics
    numbers = [1, 3, 4, 5, 7, 9, 2]
    
    x = statistics.mean(numbers)
    
    print("Mean is :", x)
    ```

### 2. Duel-of-Sorcerers

Let's go with the battle! 

The first part of this exercise it is perfect, but... What happened with the bonus? 

The first step that we should do in this exercise is extract the values (from the dictionary) of each power for each sorceress. For do this we could code: 

```python
#create two new lists where we append each value for a given value
gandalf_power = []
saruman_power = []

# then extract the values from the dictionary
for g in gandalf:
    gandalf_power.append(POWER[g]) # we get a list with each value of a given power for gandalf

for s in saruman:
    saruman_power.append(POWER[s])

# then, you should iterate between this two new list and compare each value in gandalf_power and saruman_power. 

for spell in range(spells):
    
    if gandalf_power[spell] > saruman_power[spell]:
            # to ensure that one of the Sorcerers win 3 duels it is necessaty to reset the counter 
            gandalf_wins += 1 🚨
            saruman_wins = 0 🚨
            if gandalf_wins == 3:
                print(f'Gandalf has won {gandalf_wins} clashes in a row, he is the winner of the battle!\n')
                break
            else:
                print(f"Gandalf wins this clash. It is the {gandalf_wins} victory in a row!\nSaruman's wins are reset to 0.\n")
    ... # and the other condition
```

Although they are not mandatory, it is important that we do them because they will help us to create more complex code and can be a challenge from which we will learn a lot.

### 3. Bus

Overall this part of the prework it is perfect! I have only one thing to tell you:

- In the exercise 2 *Assign to a variable a list whose elements are the number of passengers at each stop (in-out).*

    The exercise asked us to calculate the number of people on the bus at each stop. In this case, we could do:

    ```python
    passengers_at_stop = [] 
    total = 0

    for stop in stops: # iterate through the list of tuples
        #stop = each tuple of the list
        total += stop[0] - stop[1] # sum the people who get on (element zero of each tuple (stop[0])) at each stop and subtract those who get off (element one of each tuple (stop[1])).
        passengers_at_stop.append(total) #append the results in a list
    
    print (passengers_at_stop)
    ```

### 4. Robin-Hood

Good job in this challenge!!! 💪 As an interesting fact, in the exercise 1 *Robin Hood is famous for hitting an arrow with another arrow. Find the coordinates of the points where an arrow hits another arrow.* we could use the `set` python method. A Set is an unordered collection data type that is iterable, mutable and has no duplicate elements, i.e. remove duplicated values and give us only the unique values. 

### 5. Temperature-Processor

Really good job in this challenge Luisa 🔥

### 6. Rock–Paper–Scissors

Let's go with this exercise, overall it is perfect, however, there are part of the code that you could atomize. For example: 
- In the exercise 8 *Define a function that checks who won a round.* 
  The `check` function it is perfect, but we could optimize our code using the `or` and `and` operators and reduce the number of lines. It is good practice to try to avoid repeating lines of code that are too similar. One possible solution in this case could be: 

  ```python
  def game(player, pc):
    # return true is the player beats the pc
    # winning conditions: r > s, s > p, p > r
    if (choice_computer == choice_user:): 
        return 0
    elif (choice_computer == gestures[0] and choice_user == gestures[1]) or (choice_computer == gestures[1] and choice_user == gestures[2]) or (choice_computer == gestures[2] and choice_user == gestures[0]):
        return 2
    else: 
        return 1
  ```
- Suuuper you are call defined functions created before inside new functions 🔥🎉. 

- The bonus exercise was similar to rock, paper, scissors, the only thing we should do is add two more possible options. 

Still, great job Luisa!!!! You are on the data analysis rocket! 🚀
