# Neural Network Learner (MNIST) on SQL Server Machine Learning Services

This is the SQL script to generate SQL Server's table for well-know MNIST (hand-writing digits) dataset.

See [https://tsmatz.wordpress.com/2018/03/19/rxneuralnet-tutorial-for-sql-server-database/](https://tsmatz.wordpress.com/2018/03/19/rxneuralnet-tutorial-for-sql-server-database/).

## How to prepare data

1. Copy mnist_table.csv and createtable.sql
2. Run the following command, in which "C:\Demo\mnist_table.csv" must be your absolute path for mnist_table.csv

```bash
sqlcmd -U xxxxx -P P@ssw0rd -i createtable.sql -v datafile="C:\Demo\mnist_table.csv"
```

3. Run mnist_rxnuralnet.R using generated table !

Note : "bulkadmin" or "sysadmin" role is needed.
