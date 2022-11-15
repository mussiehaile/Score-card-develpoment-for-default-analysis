# Score-card-develpoment-for-default-analysis

In this project we will solve one of the prominent problems in the banking system. lending money and not be able to collect it is one of the few problems in the baking sectors.so banks try different tools to minimize the loss .one solution could be scoring every individual with some metrics and try to make decision whether to lend or not based on this score. in this project I build models that calculates the expected loss when the banks lend money to individuals. The goal of the model is to minimize the risk for the banks to make a safe loan to individuals.

Expected loss - the amount a bank may lose by lending to a borrower.

expected loss is the aggregate of three models.

1.Probability of default (pd) - tells us a which borrower might be inability to pay their dept.
2.LGD- a proportion of total exposure that can't be recovered by the banks once a default has occurred.
3.EAD - the total value that a lender is exposed to when a borrower defaults.

EL= PD + LGD +EAD

given row data there might be preprocessing unique to score card development: -

1.Fine Classing

Fine classing is applied to all continuous variables and those discrete variables with high cardinality. This is the process of initial binning into typically between 20 and 50 fine granular bins.

2.Coarse Classing

Coarse classing is where a binning process is applied to the fine granular bins to merge those with similar risk and create fewer bins, usually up to ten.

3.Dummy Coding

The process of creating binary (dummy) variables for all coarse classes except the reference class.

after this step usually training done using logistic regression.

finally developing score card so that anyone can use it.
