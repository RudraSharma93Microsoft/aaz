# [Command] _support in-subscription chat-transcript show_

Get chatTranscript details for a support ticket under a subscription.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5zdXBwb3J0L3N1cHBvcnR0aWNrZXRzL3t9L2NoYXR0cmFuc2NyaXB0cy97fQ==/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/providers/microsoft.support/supporttickets/{}/chattranscripts/{} 2022-09-01-preview -->

#### examples

- Get chatTranscript details for a support ticket under a subscription.
    ```bash
        support in-subscription chat-transcript show --support-ticket-name "TestTicketName" --chat-transcript-name "TestChatTranscriptName"
    ```
