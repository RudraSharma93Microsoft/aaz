# [Command] _support services problem-classifications show_

Get problem classification details for a specific Azure service.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3Byb3ZpZGVycy9taWNyb3NvZnQuc3VwcG9ydC9zZXJ2aWNlcy97fS9wcm9ibGVtY2xhc3NpZmljYXRpb25zL3t9/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /providers/microsoft.support/services/{}/problemclassifications/{} 2022-09-01-preview -->

#### examples

- Gets details of problem classification for Azure service.
    ```bash
        support services problem-classifications show --service-name "ServiceNameGuid" --problem-classification-name "ProblemClassificationNameGuid"
    ```
