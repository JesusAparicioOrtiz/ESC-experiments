# ESC-experiments
Experiments made with [Elastic-Smart-Contracts](https://github.com/isa-group/elastic-smart-contracts)

All experiments are divided in folders with an ID. Inside each experiment folder, there are a couple of things:
- A folder for each ESC started during the experiment. Inside these folders, there is CSV file with the following information:
  - **RESPONSE**: Number of responses returned by the analysis.
  - **TOTAL_TIME**: Time in seconds since the transaction was submitted until it returned a response.
  - **ANALYSIS_TIME**: Time in seconds of analysis transaction
  - **FREQUENCY**: Frequency of elasticity in seconds, every X seconds the system will evaluate the transaction time and will update data collection frequency or the window depending on the ESC configuration.
  - **TIME_DATA**: Window of time in seconds, every data stored in the assets before that time, will be considered as valid.
  - **FREQUENCY_DATA**: Frequency of data collection in seconds.
  - **RESPONSES_STORED**: Responses stored in the asset at the time of the analysis transaction.
  - **FROM_DATE**: Timestamp of when the analysis transaction is submitted.
  - **TO_DATE**: Timestamp of when the analysis transaction return a response.
  - **MINIMUN_TIME**: Upper threshold in seconds for elasticity evaluation.
  - **MAXIMUN_TIME**: Lower threshold in seconds for elasticity evaluation.
  - **CURRENT_ESC_RUNNING**: Number of ESC running at the time of the analysis transaction execution.
  - **ANALYSIS_RETRIES**: Number of analysis transaction submissions retries.
  - **HOOK_DATA_RETRIES**: Number of update data transaction submissions retries.
  - **INIT_EXEC_TIME**: Timestamp of when the analysis transaction is executed.
  - **FINAL_EXEC_TIME**: Timestamp of when the analysis transaction is finished.
  - **ID**: ID of the ESC analysis transaction
  - **GUARANTEES_NUMBER**: Number of guarantees calculated.
  - **METRICS_VALUES**: Metric values used to calculate the guarantees.
  - **GUARANTEES_VALUES**: Guarantees values calculated.
- (Only in recent experiments) "*Curva_Regresion*" CSV file, which gives some information about analysis executions for every ESC of the experiment in time intervals.
- (Only in recent experiments) "*Info*" CSV file, which gives the total time of execution, analysis execution time and window for every analysis in each ESC.
