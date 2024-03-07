# [Command] _support in-subscription tickets list_

List all the support tickets for an Azure subscription.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5zdXBwb3J0L3N1cHBvcnR0aWNrZXRz/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/providers/microsoft.support/supporttickets 2022-09-01-preview -->

#### examples

- List support tickets for a subscription
    ```bash
        support in-subscription tickets list
    ```

- List support tickets in open state for a subscription
    ```bash
        support in-subscription tickets list --filter "Status eq 'Open'"
    ```

- List support tickets in updating state for a subscription
    ```bash
        support in-subscription tickets list --filter "Status eq 'Updating'"
    ```

- List support tickets with a certain problem classification id for a subscription
    ```bash
        support in-subscription tickets list --filter "ProblemClassificationId eq 'problem_classification_guid'"
    ```

- List support tickets created on or after a certain date and in open state for a subscription
    ```bash
        support in-subscription tickets list --filter "CreatedDate ge 2024-01-01T22:08:51Z and Status eq 'Open'"
    ```

- List support tickets with a certain service id for a subscription
    ```bash
        support in-subscription tickets list --filter "ServiceId eq 'service_guid'"
    ```
