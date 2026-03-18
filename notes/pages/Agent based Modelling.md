tags:: PSS, ABM, Complex System Models, Green Infrastructure, Water Governance

- part of Complex System Models
- ### Methods to parameterise behavioural responses of humans empirically
	- **ER:** Expert knowledge
	- **PO:** Participant observation (researcher observe day to day life of communities)
	- Social surveys
	- Census data
	- Field or lab experiments
	- Role-playing games
	- Cluster analysis
	- Dasymetric mapping: combination of detailed spatial data with aggregated census data
	- Monte Carlo method: allow developing uncertainty distributions of output variables
	-
-
- ### Framework
  ![image.png](../assets/image_1773667056263_0.png)
  this paper focusses only on human agents and not on social networks and agent environment. So we Focus on **M1 to M5**
- | M1 | M2 | M3 | M4a ATB | M4b BT | M5 |
  |----|----|----|---------|--------|----|
  | Expert knowledge | Survey | Survey | Clustering and regression | Clustering and regression | Proportional |
  | Participant observation (ParticObser) | Census (incl. GIS data) | Interviews | Correlation and expert knowledge | Correlation + expert knowledge | Census/GIS based assignment |
  | Lab experiment | | Field experiment | Expert knowledge | Expert knowledge | Monte Carlo |
  | Interviews | | ParticObser | Dasymetric mapping | ParticObser | |
  | RPG | | RPG | | | |
  | | | Time-series data | | | |
  | | | Expert knowledge | | | |
- #### Agent Class:
	- agents that have the same sequence of method are in the same agent class
-
- | Case | N high? | Sample representative? | BD high? | M1 | M2 | M3 | M4a | M4b | M5 |
  |------|---------|----------------------|----------|----|----|----|-----|-----|----|
  | 1 | Yes | Yes | Less relevant | EK or PO or Interviews (optional: Experiments or RPG) | Survey | Interviews or Field Experiments or RPG or EK | — | — | (Cloning or Monte Carlo) and Spatial references |
  | 2 | Yes | No | Yes | EK or PO or Interviews (optional: Experiments or RPG) | Survey | Interviews or RPG | — | (EK or Clustering) and Regression | CD/GIS based |
  | 3 | Yes | No | Yes | EK or PO or Interviews (optional: Experiments or RPG) | Survey | Interviews or RPG | Clustering or (Statistics and EK) | — | CD/GIS based |
  | 4 | Less relevant | Yes | Yes | EK or PO or RPG | Census & Surveys (or PO) | Interviews (PO) or RPG | PO | PO | CD/GIS based |
  | 5 | No access | No | — | EK or PO | Disaggregated Census | Time-series data AND EK | — | EK | CD/GIS based |
  | 6 | Yes | No | No | EK or PO or Interviews (optional: Experiments or RPG) | Survey | Interviews or Field Experiments or RPG | — | (EK or Clustering) and Regression | CD/GIS based |
  | 7 | No | 100% | Less relevant | EK or PO or Interviews (optional: Experiments or RPG) | Survey | Interviews or Field Experiments or RPG | — | — | No up-scaling |
  | 8 | Yes | Less relevant | No | EK or PO or Interviews (optional: Experiments or RPG) | Survey OR Census | EK or Interviews or Field Experiments or RPG | Statistics and EK | — | CD/GIS based |
  | 9 | No | Less relevant | No | EK or PO or RPG | Census | EK or Field Experiments or RPG | EK | EK | No up-scaling |
  | 10 | No | Less relevant | Yes | EK or PO or RPG | Census | EK or RPG | EK | EK | No up-scaling |
  | 11 | Less relevant | Less relevant | Less relevant | EK or PO | Aggregated Census | Time-series data | Dasymetric mapping | Clustering & Regression | CD/GIS based |
  | 12 | Less relevant | Less relevant | Less relevant | EK or PO | Disaggregated Census | Time-series data | — | Clustering & Regression | CD/GIS based |
- [[smajglEmpiricalCharacterisationAgent2011]]
-
- ### Empirical parameterisation in practice
	- Montalto et al. explicitly follow the [[smajglEmpiricalCharacterisationAgent2011]] framework and nomenclature throughout
	- Agent classes identified via expert knowledge, semi-structured interviews (20 orgs), participant observation, surveys (~70 residents), community meetings
	- Up-scaling done via Monte Carlo draws from GIS and census distributions → matches M5 in Smajgl
- ### Agents
	- Three agent classes: water utility (PWD), community greening organisations, property owners
	- Property owner attributes: income, tenure (owner/renter), roof age, org membership — all from census + survey (M2)
- ### Adoption probability: two scenarios
	- **Scenario 1** (expert model, M3 = economic self-interest only):
		- `P = F × E`
		- F = physical feasibility gate (0 or 1)
		- E = logistic function of G, where `G = incentive / monthly income` — scales incentive to individual income
	- **Scenario 2** (empirically enriched, M3 = surveys + interviews + participant observation):
		- `P = F × E × W × K`
		- W = willingness (40% unwilling for rain gardens, 60% for green roofs — from survey)
		- K = knowledge factor: boosted by org membership, GI already on block; reduced by rental status
		- → corresponds to Smajgl Cases 1–2: large population, behavioural diversity added iteratively
- ### Key finding
	- Scenario 1 hits 30% greening goal in ~3 months; Scenario 2 takes ~5 years
	- Difference driven almost entirely by W (scepticism from surveys) — shows sensitivity of ABM outcomes to empirical grounding
	- Spatial clustering around early adopter orgs (Point Breeze Pioneers, Newbold Neighbors) visible early in Scenario 2 → community organisations matter for spatial outcomes
- [[montaltoDecentralisedGreenInfrastructure2013]]