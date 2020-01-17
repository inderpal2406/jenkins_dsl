## Table of Content

1. [simple_pipeline_1](./simple_pipeline_1): a simple pipeline with 3 stages- build, test and deploy.
2. [multi_step_pipeline](./multi_step_pipeline): a single stage pipeine with multiple steps.
3. [retry_pipeline_1](./retry_pipeline_1): a pipeline with retry block. It'll retry the block specified no of times, if it fails to execute.
4. [retry_pipeline_2](./retry_pipeline_2): a pipeline with retry block. It'll retry the block specified no of times, if it fails to execute (irrespective of fact if few commands passed and few failed in the retry block, it'll retry all commands again).
5. [timeout_pipeline_1](./timeout_pipeline_1): the step will timeout if the command takes more than a specified time interval.
6. [timeout_pipeline_2](./timeout_pipeline_2): timeout block has more than one command, and timeout will consider cumulative time for all commands, if this cumulative time exceeds than the time interval set as timeout, then the step is aborted.
7. [timeout_pipeline_3](./timeout_pipeline_3): the command before timeout block was executed, the timeout block expired after timeout and the complete job was aborted. The retry block after timeout block in first stage was not executed. Also the next stage was not executed.
