# [Command] _support in-subscription file show_

Get details of a specific file in a work space.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5zdXBwb3J0L2ZpbGV3b3Jrc3BhY2VzL3t9L2ZpbGVzL3t9/2022-09-01-preview.xml) **Preview**

<!-- mgmt-plane /subscriptions/{}/providers/microsoft.support/fileworkspaces/{}/files/{} 2022-09-01-preview -->

#### examples

- Show a file within a file-workspace for a specified subscription
    ```bash
        support in-subscription file-workspace file show --subscription "TestSubscription" --file-workspace-name "TestWorkspaceName" --file-name "FileName"
    ```
