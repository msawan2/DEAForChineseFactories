# DEAForChineseFactories

A consultancy firm advising the Chinese government on the procurement of manufactured goods, is developing a scalable mechanism for measuring the efficiency of factories across Chinese provinces.

In order to compute accuracies, Data Envelopment Analysis (DEA) was utilized, which is used to score business efficiency based upon a set of inputs and outputs for that particular business. Inputs and output for our dataset are as follows:

Inputs: Capital (in 100 million RMB), Labor (in 10,000 persons)

Output: Gross Industrial Output Value (GIOV) (in 100 million RMB)

A linear model was constructed and solved for in both Python (Pyomo) and Excel (Solver). Following are the objective function, decision variables and constraints:

Objective: Maximize the calculation of the weighted output scores to yield a solution for the linear program. The greater the output score, the higher the overall efficiency score as calculated by the output scores divided by the input scores.

Decision Variables: In the linear programming model, the decision variables were the weights used for calculating the weighted input and output scores necessary for computing the overall efficiency score for each factory.

Constraints: From within the linear optimization program, there were two constraints which were as follows:
Output_scores <= Input Scores (A factory can only produce with using the resources that it has available)
Input Scores = 1 (In DEA, there can be no efficiency score > 1)

Efficiencies were calculated and visual analysis was carried out.

Data Envelopment Analysis (DEA) is a linear programming method for measuring the efficiency of Decision Making Units (DMUs) to improve organizational performance in the private and public sectors. However, if new DMUs need to know the respective efficiency score, the DEA analysis would have to be conducted again. In today’s fast paced world where new data is generated with every second, recalculation of efficiency requires a huge amount of computation. To solve this problem, an ML model was built that measures and predicts the DEA efficiency of DMUs.

Please go through Data Envelopment Analysis (DEA) for Chinese Manufacturing Companies.pptx slides in order to understand the project in more detail.

Python (Pyomo) model is in Application_Project_DEA_EconomyLong.ipynb and Excel (Solver) model is in DEA_ApplicationProject.xlsx. 

Thank you for reading, and have a good day!
