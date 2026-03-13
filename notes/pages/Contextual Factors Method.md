## Questionnaire Summary
collapsed:: true
	- The data were collected through an international online questionnaire distributed
	  to approximately 1,300 members of the *Computers in Urban Planning and Urban
	  Management* (CUPUM) research community between May and July 2019. A total of 268
	  responses were received (response rate ≈ 20%), of which **175 were used in the
	  analysis** — those from respondents involved in smart city projects where ICT
	  played a significant role.
	- ### Structure
	  
	  The questionnaire consisted of three parts:
	  
	  1. **Respondent background:** gender, age, profession, geographical origin, and
	   level of expertise with planning support ICTs.
	  2. **PSS in practice:** perceptions of PSS application in smart city projects,
	   covering five themes — urban problems, functionalities, usability, added value,
	   and contextual factors. Responses were recorded on a **7-point Likert scale**
	   (1 = low, 7 = high).
	  3. **Conference-specific questions:** related to the 2019 CUPUM conference; not
	   used in this study.
	- ### Sample Characteristics
	  
	  | Attribute | Detail |
	  |---|---|
	  | **Geography** | China (53%), Europe (15.4%), Asia excl. China (14.2%), North America / South America / Oceania (5.1% each), Africa (2.3%) |
	  | **Profession** | Academic researchers & doctoral students (61.7%), planners (32.6%), designers (3.4%), politicians (2.3%) |
	  | **Mean PSS usefulness** | 2.90 (on a recoded ordinal scale from 1 to 5) |
-
- ## Used Logistic Model:
  collapsed:: true
	- $Y$ - usefulness
	- $X$ - contextual factors
	- fit model to: 
	  $logit (P(Y \leq j | x) = \ln \frac{ (P(Y \leq j | x)}{1 - (P(Y \leq j | x)}  = \alpha_j - \beta_{1,i}x_1 - .... - \beta_{k,i}x_k$
		- $j \in \{1,...5\}$ usefulness score
		- $k$ number of questions
		- $i$ integer answer of question $k$
		- $\alpha_j = logit (P(Y \leq j | ref)$ is the threshold for usefulness score $j$ and all values are set to their reference
		- $x_{i,k} \in \{0,1\}$
		-
		-
	- Table 3 values are estimates, so:
		- $\beta_{i,k} = logit (P(Y \leq j | x)) - a_j$
			- (log odds for usefulness being lower or equal j at x) -
			  (log odds for usefulness being lower at or equal j for ref)
			- same as log odd ratio just in a different scale
			- $OR = \frac{P(Y \leq j \mid x_k = l) / (1 - P(Y \leq j \mid x_k = l))} {P(Y \leq j \mid x_k \text{ref}) / (1 - P(Y \leq j \mid x_k = \text{ref}))}$
			- $P(Y \leq j \mid x_k = l) / (1 - P(Y \leq j \mid x_k = l))$ ratio of being smaller or equal to j to bigger than j. So one to ratio.
			- ratio of low usefulness to high usefulness under l / ratio of low usefulness to high usefulness under ref
			- example transparency:
				- Transparency = 2: 0.4 to be lower than any j
				- Transparency  = ref: 0.2 to be lower than any j
				- $\frac{0.4 / 0.6}{0.2 / 0.8} =\frac{0.6666}{0.25} = 2.4$ -> usefulness increases with higher transparency
			- example analysis:
				- Analysis = 2: 0.4 to be lower than any j
				- Analysis  = ref: 0.6 to be lower than any j
				- $\frac{0.4 / 0.6}{0.6 / 0.4} =\frac{0.6666}{1.5} = 0.4$ -> usefulness decreases with higher analysis
		- $\beta$ is a number you add to the baseline log-odds — a big positive number pushes the OR toward more useful (high value), a big negative number pushes it toward less useful (low positive value), and the size tells you how strong that push is.
		- Derivation:
			- $logit(P(Y \leq j | x)) = \alpha_j - \beta_{1,i}x_1 - .... - \beta_{k,i}x_k$
			- set all $x$ to 0, but $x_{i,k}$
			- $\Leftrightarrow  \beta_{k,i} = logit (P(Y \leq j | x)  - \alpha_j$
			- holds for all $j$
		- The p-value follows a three-step derivation:
			- Compute the **standard error** from the curvature of the log-likelihood function
			- Compute the **Wald statistic** as the squared ratio of estimate to standard error
			- Compute the **p-value** as the right-tail area of the χ²(1) distribution at that Wald value
- ---
-
- Results: [[Contextual Factors Study Results]]
- [[jiangEffectsContextualFactors2021]]