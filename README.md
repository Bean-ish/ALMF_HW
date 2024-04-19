## 4: PDP, ICE, etc.

## 5: LIME & SHAPLEY
sort the data by 1 or 2 features, separate into bins<br>
fit the model to the whole dataset<br>
<br>
**LIME**<br>
from each bin:<br>
	select N=10 samples to do LIME - local linear regression with 3 features<br>
	explain the local surrogate model<br>
overall assessment of feature importance of each bin<br>
<br>
**Shapley Value**<br>
3 features<br>
for each bin<br>
- for each feature of interest, 2^2 = 4 coalitions excluding the feature:<br>
	- for each coalition:<br>
		1. calculate the probability of joining<br>
		2. sample 10 random points and perform replacement<br>
		3. value differences<br>
		4. take average<br>
	- add them up<br>
- plot things<br>
<br>
explain across bins<br>
