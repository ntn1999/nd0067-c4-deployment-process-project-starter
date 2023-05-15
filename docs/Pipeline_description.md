Pipelines are normally written inside configuration files as a list of steps.
It contains the following sections:

    CircleCI version: This is simply indicating which version of the platform our pipeline should use.
    Orbs are a set of instructions created by CircleCi that allow us to configure the pipeline on which we will run our actions. These instructions will instruct the server to setup specific software on the server executing our pipeline. We could use orbs to setup node.js or install the AWS CLI for example. Orbs are not always present in a pipeline.
    Jobs are groups of commands that we want to run. This is where we will run commands to install, build or deploy our application.
    Workflows are instructions about the order of the jobs. They allow us to create complex flows and specify manual approvals. Workflows are not always present in a pipeline.