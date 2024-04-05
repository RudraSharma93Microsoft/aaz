# [Command] _support services list_

List all the Azure services available for support ticket creation. Always use the service and problem classifications obtained programmatically. This practice ensures that you always have the most recent set of service and problem classification Ids.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3Byb3ZpZGVycy9taWNyb3NvZnQuc3VwcG9ydC9zZXJ2aWNlcw==/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /providers/microsoft.support/services 2022-09-01-preview -->

#### examples

- Gets list of services for which a support ticket can be created.
    ```bash
        support services list
    ```
