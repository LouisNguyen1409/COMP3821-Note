**Master Theorem**

 - ***Genral Equation***

	T(n) = aT(n/b) + f(n)  
	where a >= 1, b > 1 and f(n) = O(n<sup>k</sup> (log n)<sup>P</sup>)

 - ***Cases***

	For cases, we will compare 2 variables to determine which case is it. Two variables are log<sub>b</sub>(a) and k.

	- ***Case 1: If log<sub>b</sub>(a) > k***  
	Therefore, the big-Oh will be O(n<sup>log<sub>b</sub>a</sup>)

	- ***Case 2: If log<sub>b</sub>(a) = k***

		- If P > -1, then O(n<sup>k</sup> (log n)<sup>P+1</sup>)
		- If P = -1, then O(n<sup>k</sup> log(log n))
		- If P < -1, then O(n<sup>k</sup>)

	- ***Case 3: If log<sub>b</sub>(a) < k***

		- If P >= 0, then O(n<sup>k</sup> (log n)<sup>P</sup>)
		- If P < 0, then O(n<sup>k</sup>)
 - ***Example***

	[Youtube Example](https://www.youtube.com/watch?v=kGcO-nAm9Vc&ab_channel=AbdulBari)