## Table of Content

1. [simple_pipeline_1](./simple_pipeline_1): a simple pipeline with 3 stages- build, test and deploy.
2. [multi_step_pipeline](./multi_step_pipeline): a single stage pipeine with multiple steps.
3. [retry_pipeline_1](./retry_pipeline_1): a pipeline with retry block. It'll retry the block specified no of times, if it fails to execute.
4. [retry_pipeline_2](./retry_pipeline_2): a pipeline with retry block. It'll retry the block specified no of times, if it fails to execute (irrespective of fact if few commands passed and few failed in the retry block, it'll retry all commands again).
5. [retry_pipeline_3](./retry_pipeline_3): command before retry block was executed, retry block was retried for 3 times due to failures, command after retry block in retry stage was not executed, and after-retry stage was skipped due to failures in previous stage.
6. [timeout_pipeline_1](./timeout_pipeline_1): the step will timeout if the command takes more than a specified time interval.
7. [timeout_pipeline_2](./timeout_pipeline_2): timeout block has more than one command, and timeout will consider cumulative time for all commands, if this cumulative time exceeds than the time interval set as timeout, then the step is aborted.
8. [timeout_pipeline_3](./timeout_pipeline_3): the command before timeout block was executed, the timeout block expired after timeout and the complete job was aborted. The retry block after timeout block in first stage was not executed. Also the next stage was not executed.
9. [env_var_pipeline](./env_var_pipeline): how to set env vars for a job in jenkins using pipeline-as-code practices.
10. [creds_pipeline](./creds_pipeline): to demonstrate handling of secrets in pipeline code.
11. [post_action_pipeline](./post_action_pipeline): to demonstrate post actions in pipeline.
12. [dummy_complete_pipeline](./dummy_complete_pipeline): a demo pipeline with Build, Test, Push, Deploy stages.
