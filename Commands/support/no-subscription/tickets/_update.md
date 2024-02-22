# [Command] _support no-subscription tickets update_

Update API allows you to update the severity level, ticket status, advanced diagnostic consent, secondary consent, and your contact information in the support ticket.<br/><br/>Note: The severity levels cannot be changed if a support ticket is actively being worked upon by an Azure support engineer. In such a case, contact your support engineer to request severity update by adding a new communication using the Communications API.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3Byb3ZpZGVycy9taWNyb3NvZnQuc3VwcG9ydC9zdXBwb3J0dGlja2V0cy97fQ==/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /providers/microsoft.support/supporttickets/{} 2022-09-01-preview -->

#### examples

- Update support ticket severity.
    ```bash
        support no-subscription tickets update --support-ticket-name "TestTicketName" --severity "moderate"
    ```

- Update support ticket status.
    ```bash
        support no-subscription tickets update --support-ticket-name "TestTicketName" --status "closed"
    ```

- Update support ticket customer contact details properties
    ```bash
        support no-subscription tickets update --support-ticket-name "TestTicketName" --contact-additional-emails "xyz@contoso.com" "devs@contoso.com" --contact-country "USA" --contact-email "abc@contoso.com" --contact-first-name "Foo" --contact-language "en-US" --contact-last-name "Bar" --contact-method "phone" --contact-phone-number "123-456-7890" --contact-timezone "Pacific Standard Time"
    ```

- Update advanced diagnostic consent of a support ticket
    ```bash
        support no-subscription tickets update --support-ticket-name "TestTicketName" --diagnostic-consent "Yes"
    ```

- Update secondary consent of a support ticket
    ```bash
        support no-subscription tickets update --support-ticket-name "TestTicketName" --secondary-consent "[{type:VirtualMachineMemoryDump,user-consent:No}]"
        support no-subscription tickets update --support-ticket-name "TestTicketName" --secondary-consent [0].type="VirtualMachineMemoryDump" [0].user-consent="No"
        support no-subscription tickets update --support-ticket-name "TestTicketName" --secondary-consent [0]="{type:VirtualMachineMemoryDump,user-consent:No}"
    ```
