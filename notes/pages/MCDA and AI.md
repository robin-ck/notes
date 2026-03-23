- **# MCDA meets AI: a comprehensive literature map (2021–2026)**
  
  The integration of Multi-Criteria Decision Analysis (MCDA) with Artificial Intelligence and Machine Learning has accelerated dramatically since 2021, producing a rich and rapidly expanding body of literature across every major application domain. **The landmark review by Liao et al. (2023) in *Information Fusion*** established the first comprehensive map of this intersection****, identifying four core ML contributions to MCDM: criteria extraction, criteria interaction modeling, parameter determination, and integrated solution generation. Across five domains—general frameworks, environmental/sustainability, engineering/infrastructure, business/finance, and healthcare—researchers have developed hybrid methodologies that leverage MCDA's transparent structure alongside AI's predictive power. Two dominant integration paradigms have emerged: ML enhancing MCDA (automated weighting, data-driven criteria, handling incomplete data) and MCDA evaluating ML (model selection, algorithm benchmarking, explainability). This report catalogs the most significant papers, methodologies, and trends across all domains.
  
  ---
  
  **## Meta-reviews and bibliometric analyses anchor the field**
  
  Several high-quality reviews and bibliometric studies published between 2021 and 2026 provide the intellectual scaffolding for this hybrid field. These are essential starting points for any researcher entering the MCDA+AI space.
  
  **Liao, H., He, Y., Wu, X., Wu, Z., & Bausys, R. (2023).** "Reimagining Multi-Criterion Decision Making by Data-Driven Methods Based on Machine Learning: A Literature Review." *Information Fusion*, 100, 101970. This is the **most cited and comprehensive review** of ML-MCDM integration, published in a journal with an impact factor exceeding 17. It conducts bibliometric analysis of research hotspots and reviews ML applications to four key MCDM challenges. It covers applications spanning business management, industrial engineering, sustainable development, and emergency management, and identifies that no prior comprehensive review of ML technologies applied to MCDM existed.
  
  **Sotoudeh-Anvari, A. (2022).** "The Applications of MCDM Methods in COVID-19 Pandemic: A State of the Art Review." *Applied Soft Computing*, 126, 109238. Reviews MCDM methods (AHP, TOPSIS, VIKOR, PROMETHEE) applied to pandemic decision problems including treatment selection, hospital resource allocation, vaccine distribution, and public health policy, with discussion of AI/ML integration approaches.
  
  **Torkayesh, A.E. et al. (2022).** "Review of Multi-Criteria Decision-Making Methods in Finance Using Explainable Artificial Intelligence." *Frontiers in Artificial Intelligence*, 5, 827584. Bridges MCDM and explainable AI (XAI) for finance, arguing that MCDM's inherent transparency can complement AI's predictive power while maintaining auditability—a framework applicable well beyond finance.
  
  **Kumar, R. & Pamucar, D. (2025).** "A Comprehensive and Systematic Review of Multi-Criteria Decision-Making Methods: Two Decades from 2004 to 2024." *Spectrum of Decision Making and Applications*, 2(1), 177–196. Bibliometric analysis using VOSviewer on **3,655 peer-reviewed articles**, documenting MCDM's transformation from foundational methods into dynamic hybrid models integrating AI, fuzzy logic, and ML.
  
  **Sahoo, S.K. & Goswami, S.S. (2023).** "A Comprehensive Review of Multiple Criteria Decision-Making Methods: Advancements, Applications, and Future Directions." *Decision Making Advances*, 1(1), 25–48. Critically analyzes data-driven and ML-based MCDM models, noting they require large datasets and computational resources but enable real-time, large-scale decision-making.
  
  **Ali, R., Hussain, A., Nazir, S., Khan, S., & Khan, H.U. (2023).** "Intelligent Decision Support Systems—An Analysis of Machine Learning and Multicriteria Decision-Making Methods." *Applied Sciences* (MDPI), 13(22), 12426. Part of a special issue on "Multi-Criteria Decision Making Using Artificial Intelligence," this paper analyzes synergistic ML-MCDM combinations across business, healthcare, education, and industry.
  
  **Taherdoost, H. & Madanchian, M. (2023).** "Multi-Criteria Decision Making Methods and Concepts." *Encyclopedia* (MDPI), 3(1), 77–87. Documents the field's exponential growth at **14.18% annual increase** with 33,201 authors across 131 countries. AHP remains the most popular method, followed by TOPSIS, VIKOR, PROMETHEE, and ANP.
  
  Additional domain-specific reviews include: **de Santana Filho et al. (2025)** on MCDA-AI in circular economy and reverse supply chains (*Applied Sciences*, 15(9), 4758); a **GIS+AI+MCDA comprehensive review (2025)** for sustainable urban planning (*Applied Spatial Analysis and Policy*, Springer); **Reyes-Norambuena et al. (2025)** on ML+MCDA for pedestrian modeling (*Sustainability*, 17(1), 41); and **Sutiene et al. (2024)** on AI and MCDM for portfolio management (*Frontiers in Artificial Intelligence*, 7, 1371502).
  
  ---
  
  **## General and domain-agnostic hybrid frameworks**
  
  Domain-agnostic papers proposing novel MCDA+AI architectures represent the methodological core of this field. The most notable contributions introduce transferable frameworks rather than application-specific solutions.
  
  **Guo, S., Zhang, K., Liao, H., Chen, G., & Zeng, X. (2021).** "A Hybrid Machine Learning Framework for Analyzing Human Decision-Making Through Learning Preferences." *Omega* (Elsevier). Proposes **NN-MCDA**, combining an additive value model with a deep neural network—a linear component for explicit non-monotonic attribute relationships and a nonlinear MLP for implicit high-order interactions. Validated on three real-world datasets, this paper demonstrates improved MCDA prediction using ML while enhancing ML interpretability using MCDA.
  
  **Maghsoodi, A.I., Torkayesh, A.E., Wood, L.C., Herrera-Viedma, E., & Govindan, K. (2023).** "A Machine Learning Driven Multiple Criteria Decision Analysis Using LS-SVM Feature Elimination." *Engineering Applications of Artificial Intelligence*, 119. Introduces LS-SVM-driven MCDA for sustainability assessment with incomplete data, demonstrating how ML can preprocess and handle missing values that traditionally hinder multi-criteria analysis.
  
  **Nafei, A. et al. (2024).** "Smart TOPSIS: A Neural Network-Driven TOPSIS with Neutrosophic Triplets for Green Supplier Selection." *Expert Systems with Applications*, 255, 124744. Introduces **"Smart TOPSIS"**—a neural network-driven extension of classical TOPSIS using neutrosophic triplets for handling indeterminate information. Though demonstrated on supplier selection, the framework is designed as a generalizable methodology.
  
  **Torkayesh, A.E. et al. (2024).** "A Novel ML-MCDM-Based Decision Support System for Evaluating Autonomous Vehicle Integration Scenarios." *Artificial Intelligence Review* (Springer). Integrates Random Forest with **three novel MCDM algorithms** (ME-ARWEN, Compromiser-PNN, CWP) and provides open-source Python implementation—one of the few papers offering reproducible ML-MCDM software.
  
  **Tian, Z., Liang, H., Nie, R., Wang, X., & Wang, J. (2023).** "Data-Driven Multi-Criteria Decision Support Method for Electric Vehicle Selection." *Computers & Industrial Engineering*, 177, 109061. Replaces subjective MCDM inputs with ML-derived, data-driven parameters for criteria weights and performance scores, establishing a general template for modernizing any MCDM application.
  
  **Nori Alsaedi, A.G. et al. (2024).** "A Novel Framework for Intelligent Decision-Making." *International Journal of Mathematical Modelling & Computations*, 14(2), 171–186. Combines MCDA with **Deep Reinforcement Learning (DRL)**, using Q-learning simulation to show how MCDA's structured evaluation and DRL's adaptive learning from dynamic environments can complement each other.
  
  **Xue, H., Zhao, B., Xie, H., & Sun, Z. (2026).** "RankLLM: A Multi-Criteria Decision-Making Method for LLM Performance Evaluation in Sentiment Analysis." *Chinese Computational Linguistics (CCL 2025)*, LNCS 16052 (Springer). Represents the **frontier of MCDA+AI integration**, applying entropy-TOPSIS to evaluate and rank large language models—a meta-level framework where MCDA evaluates cutting-edge AI systems.
  
  Two additional framework papers target MCDA for AI method selection specifically: **Gerschütz et al. (2024)** propose a PROMETHEE-based framework for ML algorithm selection in product development (*Proceedings of the Design Society*, DESIGN 2024), and an **MDPI MAKE paper (2025)** uses 10 MCDM methods with Borda Count aggregation for selecting explainable AI methods.
  
  ---
  
  **## Environmental and sustainability applications lead in volume**
  
  The environmental domain produces the highest volume of MCDA+AI hybrid papers, driven by the inherently multi-criteria nature of sustainability assessments and the availability of geospatial data.
  
  **GIS-MCDA-ML integration dominates.** The most common pattern combines GIS spatial analysis, AHP-based criteria weighting, and ML classifiers for susceptibility mapping. Key examples include: **Nachappa et al. (2020, heavily cited through 2024)** in *Journal of Hydrology* using Random Forest + AHP + Dempster-Shafer theory for flood susceptibility; **AHP+ANN for soil erosion assessment (2025)** in *Scientific Reports* achieving 86.3% accuracy; and **AHP+LSTM for groundwater forecasting (2022)** in *Scientific Reports* combining spatial multi-criteria analysis with temporal deep learning for 5-year ahead predictions.
  
  **Renewable energy siting and planning** represents a major application cluster. A notable 2026 paper in *Energies* introduces a dynamic framework combining **LSTM deep learning for energy forecasting with Interval-Valued Pythagorean Fuzzy BWM-TOPSIS** for real-time renewable energy decision support in smart cities. **TOPSIS+Random Forest/LightGBM** for hybrid energy management appears in *Electric Power Systems Research* (2022), and **GIS-AHP+Linear Regression** for solar/wind farm siting appears in *Sustainability* (2023).
  
  **Circular economy and waste management** is an emerging sub-field. **De Santana Filho et al. (2025)** conduct a PRISMA-guided systematic review in *Applied Sciences* of hybrid MCDA-AI models (TOPSIS, AHP, neural networks, genetic algorithms) for reverse supply chain solid waste management, finding that these hybrids enhance decision-making automation and improve waste traceability.
  
  Additional important contributions include:
- **BP Neural Network + AHP for landscape ecological planning** (*Computational Intelligence and Neuroscience*, 2022)
- **PSR model + AHP + BP Neural Network for urban wetland health** (*Frontiers in Ecology and Evolution*, 2022), where the neural network identifies the 8 most significant indicators from 45 AHP-weighted candidates
- **AHP+ML classifiers for agricultural land suitability** (*Environment, Development and Sustainability*, 2023), with Balanced Bagging achieving **97.69% accuracy**
- **Fuzzy AHP + ML ensemble (RF, XGBoost, CatBoost) + Bayesian Networks for risk assessment** in power plants (*Scientific Reports*, 2025)
- **ANN + AHP + BWM + HOMER for renewable energy in healthcare facilities** (*Results in Engineering*, 2026), achieving **91.95% renewable share**
  
  The **three dominant integration patterns** in this domain are: (a) MCDA provides criteria weights, ML handles prediction/classification; (b) ML generates forecasts, MCDA performs final ranking/selection; and (c) parallel integration where both inform decision-making simultaneously.
  
  ---
  
  **## Engineering and infrastructure: from supply chains to smart cities**
  
  Engineering applications concentrate on supply chain optimization, construction management, risk assessment, and Industry 4.0 decision-making.
  
  **Supply chain and supplier selection** is the most active sub-domain. **Wyrembek & Baryannis (2024)** in *Logforum* propose two hybrid approaches—Decision Tree+AHP and FUCOM+TOPSIS+Decision Tree—achieving F1 scores of 72.57% with >5% improvement over ML-only methods while maintaining explainability. A 2024 paper in *Computers & Industrial Engineering* combines **SVM + MARCOS MCDM + Multi-Objective Mixed Integer Programming** for pharmaceutical supply chain reliability. **SVM + Fuzzy BWM + Fuzzy TOPSIS** for green supplier evaluation appears in *Applied Soft Computing* (2021), using SVM to screen core evaluation criteria from data, reducing subjectivity.
  
  **Construction management** features several innovative frameworks. **Wang, K. et al. (2023)** in *Sustainability* investigate AI technology prioritization for construction using **Delphi+Fuzzy ANP+Fuzzy TOPSIS**. A 2025 paper in Springer develops an **AI-facilitated Value Management System (AIVMS)** integrating predictive analytics, dynamic MCDM (AHP, ANP, TOPSIS), and XAI, validated through a three-round Delphi study with 24 construction professionals. A 2024 *Expert Systems with Applications* review covers intelligent DSS in construction integrating IoT, XAI, and MCDM.
  
  **Risk assessment** papers bridge engineering with AI effectively. The **Fuzzy AHP + multiple ML algorithms (RF, XGBoost, CatBoost, CNN, SVM, KNN) + Bayesian Network** framework in *Scientific Reports* (2025) uses HAZOP-derived data comprising 160 deviations and compares ensemble methods against traditional ML for process safety. **Zabihi et al. (2023)** in *International Journal of Disaster Risk Reduction* develop a smart sustainable system integrating AI with MCDM for flood damage management in infrastructure.
  
  **Manufacturing and Industry 4.0** applications include: **Fuzzy TOPSIS for Industry 4.0 technology evaluation** (*Process Integration and Optimization for Sustainability*, 2025); **Grey TOPSIS + COPRAS-G for smart manufacturing drivers** (*Benchmarking*, 2021); and multiple papers on sustainable material selection using hybrid MCDM frameworks.
  
  Notable methodological contributions include **Guo et al.'s NN-MCDA (2021)** in *Omega*, which provides a theoretical foundation applicable across engineering domains, and preference learning approaches that combine neural network pattern recognition with MCDA's structured evaluation logic.
  
  ---
  
  **## Business and finance: credit risk, ESG, and portfolio construction**
  
  Financial applications showcase some of the most sophisticated MCDA+AI integrations, particularly in credit risk assessment, ESG-driven investing, and supplier evaluation.
  
  **Credit risk assessment** represents a mature application area. **Xi, H. et al. (2022)** in *Advances in Multimedia* propose an **improved AHP + LSTM** hybrid for individual credit risk, where AHP structures the index hierarchy and LSTM captures nonlinear temporal patterns, outperforming standalone Random Forest and Wide-and-Deep models on LendingClub data. **Sun, Y. et al. (2025)** in *Complexity* introduce the first study combining **NLP-based feature extraction + AHP-CRITIC weighting + MLP + Gaussian Mixture Model** for credit risk, using both subjective (AHP) and objective (CRITIC) weighting methods. **Li, Q. (2025)** combines AHP + BP Neural Network for P2P lending risk at ICFMDE 2025.
  
  **ESG and sustainable finance** is the fastest-growing sub-area. **Sajadi et al. (2025)** in *Computational Economics* employ **TOPSIS for ESG-aware stock screening + LSTM/CNN for return prediction + Mean-Variance optimization**, demonstrating that MCDM+DL portfolios achieve the **highest Sharpe and Sortino ratios** on S&P 500 data (2010–2023). **Martínez-Barbero et al. (2026)** in *International Journal of Data Science and Analytics* combine LSTM prediction with genetic algorithms for multi-objective ESG portfolio optimization on IBEX 35 and EURO STOXX 50. ML-based ESG rating explainability research in *Annals of Operations Research* (2023) uses decision trees, Random Forest, and XGBoost to reverse-engineer Refinitiv's opaque multi-criteria ESG scoring process.
  
  **Performance evaluation and business analytics** feature novel AI-MCDM integrations. **Pinar, A. (2025)** in *Applied AI Letters* proposes a framework integrating **NLP sentiment analysis of 8,000+ customer reviews with q-Rung Orthopair Fuzzy MCDM** for retailer evaluation—a compelling example of AI-generated inputs feeding into structured MCDM. The **PROMETHEE II framework for distress prediction model evaluation** by Mousavi, M.M. & Lin, J. (2020, *Expert Systems with Applications*, extensively cited 2021–2025) establishes the paradigm of using MCDM to rank competing ML models across multiple performance criteria.
  
  **Supplier selection in Industry 4.0/5.0** contexts has generated substantial work. **Tavana et al. (2023)** in *Annals of Operations Research* integrate **Fuzzy BWM + Fuzzy Inference System** for circular supply chain supplier evaluation. **Ghanavati-Nejad et al. (2025)** in *Environment, Development and Sustainability* propose a novel **Lexicographic Goal Programming-based Stochastic BWM + ML** hybrid for viable supplier selection in automotive industry. **Lo, H.-W. (2023)** in *Advanced Engineering Informatics* develops a data-driven ML+MCDM DSS for sustainable supplier evaluation in Industry 5.0.
  
  ---
  
  **## Healthcare and medicine: diagnosis, treatment, and pandemic response**
  
  Healthcare MCDA+AI integration primarily follows two patterns: using MCDM to select optimal ML models for clinical tasks, and combining ML-based diagnosis with MCDM-based treatment recommendation.
  
  **MCDM for ML model selection in clinical diagnosis** is the dominant paradigm. **Chowdhury et al. (2022)** in *Computers in Biology and Medicine* use **TOPSIS + Entropy weighting** to select the best ML ensemble for COVID-19 cough classification, with Extra-Trees achieving AUC of **0.95** across four datasets. **Mustapha et al. (2022)** in *Diagnostics* combine supervised ML (SVM, KNN, Naive Bayes, RF, etc.) with **PROMETHEE** for breast cancer screening, ranking SVM highest. **Kumar & Kaur (2024)** in *Journal of Intelligent & Fuzzy Systems* evaluate 15 ML techniques for heart disease prediction using **CoCoSo MCDM**, and separately propose a **WSM+TOPSIS+VIKOR fusion** framework for diabetes prediction (*International Journal of Engineering and Technology Innovation*, 2024).
  
  **Integrated diagnosis-to-treatment systems** represent a more sophisticated integration. **Yaselaini et al. (2024)** in *Computers and Industrial Engineering* develop a **Diagnostic and Decision Support System (D&DSS)** combining ensemble CNNs (ResNet50V2, ResNet101V2, ResNet152V2) for psoriasis detection with MCDM for treatment recommendation—one of the few truly end-to-end hybrid systems. **Sharma et al. (2023)** in *Journal of Imaging* integrate deep learning with meta-heuristic optimization and MCDM for thyroid cancer detection from ultrasound and histopathological images.
  
  **Pandemic response** generated a surge of MCDA+AI work. A notable 2026 paper in *Scientific Reports* develops a multi-phase hybrid DSS using **K-means clustering + CRITIC weighting + three MCDM methods (MACONT, CoCoSo, EDAS)** to evaluate vaccination performance across **143 countries**. **Sotoudeh-Anvari's (2022)** comprehensive review in *Applied Soft Computing* documents the full landscape of MCDM applications to COVID-19, while the *Artificial Intelligence Review* (2022) examines MCDM+AI for pandemic medical treatment decisions.
  
  Additional notable healthcare papers include:
- **Hoda & Mondal (2023)** provide a dedicated literature survey on MCDM+ML in healthcare systems (*Journal of Artificial Intelligence and Technology*, 3(2))
- **Fuzzy AHP + Fuzzy TOPSIS for healthcare data analytics selection** (*BMC Medical Informatics and Decision Making*, 2024)
- **Fuzzy AHP + Fuzzy TOPSIS + ML (SVM, KNN, DT) for PCOS/hormonal imbalance diagnosis** (*Computers in Biology and Medicine*, 2024), where fuzzy TOPSIS outperformed ML methods
- **MCDM-MOORA for depression intervention** (*Annals of General Psychiatry*, 2024)
- **AI-driven MCDM for elderly care personalization** using CTGAN for synthetic data (*Expert Systems with Applications*, 2025)
- **TOPSIS + VIKOR + PROMETHEE II integrated with network meta-analysis** for treatment selection (*Medical Decision Making*, 2023)
  
  ---
  
  **## Cross-cutting trends, integration patterns, and research gaps**
  
  Five **integration patterns** recur across all domains:
- **Pattern 1 — MCDM weights, ML predicts**: AHP/BWM determines criteria weights; ML models use weighted features for prediction (credit risk, environmental susceptibility mapping)
- **Pattern 2 — ML reduces, MCDM ranks**: ML handles dimensionality reduction or feature selection; MCDM provides structured final ranking (supplier selection, model benchmarking)
- **Pattern 3 — MCDM evaluates ML**: PROMETHEE/TOPSIS/CoCoSo rank competing ML models across multiple performance criteria (healthcare diagnosis, distress prediction)
- **Pattern 4 — AI generates inputs, MCDM decides**: NLP/sentiment analysis or neural networks generate criteria scores; fuzzy MCDM aggregates for evaluation (retailer evaluation, dynamic energy planning)
- **Pattern 5 — Deep hybrid architectures**: End-to-end systems combining ML diagnosis with MCDM treatment recommendation, or reinforcement learning with MCDA (psoriasis D&DSS, NN-MCDA)
  
  The **most frequently combined MCDM methods** are TOPSIS (most popular), AHP (especially with fuzzy extensions), PROMETHEE, VIKOR, BWM, and emerging methods like MARCOS, EDAS, and CoCoSo. The **most frequently combined AI/ML methods** are Random Forest, neural networks (MLP, LSTM, CNN), SVM, XGBoost/gradient boosting, decision trees, and emerging LLM-based approaches.
  
  Several **research gaps** emerge from the literature. First, truly domain-agnostic, validated, general-purpose hybrid MCDA+AI frameworks remain rare—most papers demonstrate frameworks on specific case studies even when designed for transferability. Second, the integration of MCDA with generative AI and large language models is in its earliest stages, with only the RankLLM paper (2026) representing this frontier. Third, **reproducibility remains problematic**: only Torkayesh et al. (2024) provide open-source implementation code. Fourth, handling real-time, streaming data within MCDA+AI frameworks is underexplored outside energy management. Fifth, the explainability advantages of MCDA as a complement to black-box AI have been theorized (Torkayesh et al., 2022) but insufficiently validated empirically. Finally, geographic disparities persist: China, India, Iran, Turkey, and Europe dominate contributions, with limited work from Africa, Latin America, and Southeast Asia.
  
  **## Conclusion**
  
  The MCDA+AI field has matured significantly since 2021, evolving from isolated hybrid experiments into a recognized research stream with its own reviews, bibliometric analyses, and methodological identity. The most impactful development is the **bidirectional integration paradigm**—ML enhancing MCDA and MCDA evaluating ML—which creates a productive symbiosis between structured decision logic and data-driven intelligence. The field's next frontier lies in three directions: integration with generative AI and LLMs, development of validated general-purpose software frameworks with open-source implementations, and empirical demonstration that MCDA-based explainability meaningfully improves trust in AI-assisted decisions. For researchers entering this space, the Liao et al. (2023) *Information Fusion* review serves as the definitive starting point, while domain-specific entry points include Sotoudeh-Anvari (2022) for healthcare/pandemic, Torkayesh et al. (2022) for finance/XAI, and de Santana Filho et al. (2025) for sustainability/circular economy.