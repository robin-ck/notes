- > PSS usefulness is not determined by technology alone. Contextual factors — especially **transparency**, **user attitude**, **active uptakers**, and **political context** — play a decisive role. Only when PSS users can identify favorable and unfavorable contextual factors will the full potential of PSS for spatial planning be realized.
- | Contextual Factor    | Direction    | Significant?       |
  |----------------------|--------------|--------------------|
  | Transparency         | ➕ Positive  | ✅ Yes             |
  | Communicating        | ➕ Positive  | ✅ Yes             |
  | Informing            | ➕ Positive  | ✅ Yes (partially) |
  | Analyzing            | ➖ Negative  | ✅ Yes (partially) |
  | Designing            | ➖ Negative  | ✅ Yes (partially) |
  | Flexibility          | ➖ Negative  | ✅ Yes (partially) |
  | User-friendliness    | —            | ❌ No              |
  | Interactivity        | —            | ❌ No              |
  | User attitude        | ➕ Positive  | ✅ Yes             |
  | Expertise level      | ➖ Negative  | ✅ Yes (partially) |
  | Profession           | —            | ❌ No              |
  | Active uptaker       | ➕ Positive  | ✅ Yes (partially) |
  | Time pressure        | —            | ❌ No              |
  | Funding              | —            | ❌ No              |
  | Planning style (closed) | ➕ Positive | ✅ Yes            |
  | Political pressure   | ➖ Negative  | ✅ Yes             |
  | Types of urban issues | —           | ❌ No              |
-
- Used Logistic Model:
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
-
- [[jiangEffectsContextualFactors2021]]