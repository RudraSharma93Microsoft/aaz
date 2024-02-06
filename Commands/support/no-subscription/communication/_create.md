# [Command] _support no-subscription communication create_

Adds a new customer communication to an Azure support ticket.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3Byb3ZpZGVycy9taWNyb3NvZnQuc3VwcG9ydC9zdXBwb3J0dGlja2V0cy97fS9jb21tdW5pY2F0aW9ucy97fQ==/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /providers/microsoft.support/supporttickets/{}/communications/{} 2022-09-01-preview -->

#### examples

- Adds a new customer communication to an Azure support ticket.
    ```bash
        support no-subscription communication create --support-ticket-name "TestTicketName "--communication-name "TestTicketCommunicationName" --body "TicketCommunicationBody" --subject "TicketCommunicationSubject"
    ```