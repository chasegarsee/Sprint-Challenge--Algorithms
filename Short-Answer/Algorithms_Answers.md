Add your answers to the Algorithms exercises here.

a) a = 0
\*\*\* a=0 Has a constant Runtime that is determined by the amount of times it runs at its worst performance. In this case a = 0 is O(1) \*\*\*

    while (a < n * n * n): *** this is O(n**3) ***
      a = a + n * n *** since we are assigning a to a + n * n, it only runs once ***

    1 + 1 * n**3

    ***we can pair the duplicates***
    1 * n**3

    *** only the biggest number matters ***

    0(n**3)

```
b)  sum = 0 *** 0(1) *** (1)
    for i in range(n):
      i += 1 *** 0(1) *** (2)
      for j in range(i + 1, n): (3)
        j += 1 *** 0(1) *** (4)
        for k in range(j + 1, n): (5)
          k += 1 *** 0(1) *** (6)
          for l in range(k + 1, 10 + k): (7)
            l += 1 *** 0(1) *** (8)
            sum += 1 *** 0(1) *** (9)

```

    \*\*\* sum = 0, i+= 1, j+= 1, k+= 1, l+= 1, Have a constant Runtime that is determined by the amount of times it runs at its worst performance. therefore they are all O(1) \*\*\*

    As shown above, the last loop with run 9 times.
    Each loop will run n - 1 times.

    1 + n*(1 + (n - (i+1))*(1 + n - (j+1)) * 1

    *** Can get get rid of the  * 1 because its just multiplying it by 1 ***

     n*((n - (i+1))*(n - (j+1))
    [1] [2]         [3]
    *** only the biggest number matters ***

    O(n**3)


    c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)

      ***i think regardless of what is going on here, as in the above solutions, constants or assigned values always resolve to O(1)***

    O(1)
