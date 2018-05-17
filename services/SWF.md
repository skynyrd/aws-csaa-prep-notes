* Simple Workflow Service
* Workers are programs that interact with SWF to get tasks, process received tasks, and return the results
* Decider is a program that controls the coordination of tasks, i.e. their ordering, concurrency and scheduling
* Workers and the decider can run on cloud such as Amazon EC2.
* At the same time, Amazon SWF stores tasks, assigns them to workers when they are ready and monitors their progress.
* It ensures that a task is assigned ONLY ONCE and NEVER DUPLICATED.
* Workers and deciders don't have to keep the track of execution state. They can run independently, and scale quickly.
* Your workflow and activity types and the workflow execution itself are all scoped to a domain. Domains isolate a set of types, executions, and task lists from others within the same account.
* You can register a domain by using the AWS Management Console or by using the RegisterDomain action in the Amazon SWF API.
* Workflow can be 1 year ant the value is always measured in seconds.
* SWF - Task oriented API
* SQS - Message oriented API
* SWF keeps track of all the tasks and events in an application. With Amazon SQS, you need to implement your own application level tracking, especially if your application uses multiple queues.

```json
https://swf.us-east-1.amazonaws.com

{
    "name":"987987979",
    "description":"music",
    "workflowExecutionRetentionPeriodInDays":"60"
}
```