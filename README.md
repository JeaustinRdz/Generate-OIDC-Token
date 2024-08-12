# Generate-OIDC-Token
This example is how to generate an OIDC token using azure DevOps and pipelines 

# Documentation Used in the example:

API documentation: https://learn.microsoft.com/en-us/rest/api/azure/devops/distributedtask/oidctoken/create?view=azure-devops-rest-7.1#taskhuboidctoken

PreDefine Variables documentation: https://learn.microsoft.com/en-us/azure/devops/pipelines/build/variables?view=azure-devops&tabs=yaml

BuildService Account scope: https://learn.microsoft.com/en-us/azure/devops/pipelines/process/access-tokens?view=azure-devops&tabs=yaml#job-authorization-scope

# Variables used in the example:
$(System.AccessToken) = Token generated for every run by the build identity, if you have a lack of permissions you need to review the identity Project Collection Build Service ({OrgName})

$(System.TeamProjectId) = Project GUID required by the api

$(System.PlanId) = A string-based identifier for a single pipeline run.

$(System.JobId) = A unique identifier for a single attempt of a single job. The value is unique to the current pipeline.


# More information:

This documentation have an yaml example to generate an OIDC token using powershell script and predefine variables to guarantee the security and an easier automation

