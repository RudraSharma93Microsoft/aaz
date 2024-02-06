# [Command] _support no-subscription chat-transcript show_

Get chatTranscript details for a no subscription support ticket.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3Byb3ZpZGVycy9taWNyb3NvZnQuc3VwcG9ydC9zdXBwb3J0dGlja2V0cy97fS9jaGF0dHJhbnNjcmlwdHMve30=/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /providers/microsoft.support/supporttickets/{}/chattranscripts/{} 2022-09-01-preview -->

#### examples

- Get chatTranscript details for a support ticket
    ```bash
        support no-subscription chat-transcript show --support-ticket-name "TestTicketName" --chat-transcript-name "TestChatTranscriptName"
    ```