# [Command] _support in-subscription file list_

List all the Files information under a workspace for an Azure subscription.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5zdXBwb3J0L2ZpbGV3b3Jrc3BhY2VzL3t9L2ZpbGVz/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/providers/microsoft.support/fileworkspaces/{}/files 2022-09-01-preview -->

#### examples

- List all the files within a file-workspace for a specified subscription (different from the account subscription)
    ```bash
        support in-subscription file-workspace file list --file-workspace-name "TestFileWorkspaceName" --subscription "TestSubscription"
    ```

- List all the files within a file-workspace for a specified subscription (same as the account subscription)
    ```bash
        support in-subscription file-workspace file list --file-workspace-name "TestFileWorkspaceName"
    ```
