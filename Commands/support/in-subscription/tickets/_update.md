# [Command] _support in-subscription tickets update_

Updates severity level, status, advanced diagnostic consent, secondary consent, and customer contact information for a support ticket.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5zdXBwb3J0L3N1cHBvcnR0aWNrZXRzL3t9/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/providers/microsoft.support/supporttickets/{} 2022-09-01-preview -->

#### examples

- Update support ticket severity.
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --severity "moderate"
    ```

- Update support ticket status.
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --status "closed"
    ```

- Update support ticket customer contact details properties
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --contact-additional-emails "xyz@contoso.com" "devs@contoso.com" --contact-country "USA" --contact-email "abc@contoso.com" --contact-first-name "Foo" --contact-language "en-US" --contact-last-name "Bar" --contact-method "phone" --contact-phone-number "123-456-7890" --contact-timezone "Pacific Standard Time"
    ```

- Update advanced diagnostic consent of a support ticket
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --diagnostic-consent "Yes"
    ```

- Update secondary consent of a support ticket
    ```bash
        support in-subscription tickets update --ticket-name "TestTicketName" --secondary-consent "[{type:VirtualMachineMemoryDump,user-consent:No}]"
        support in-subscription tickets update --ticket-name "TestTicketName" --secondary-consent [0].type="VirtualMachineMemoryDump" [0].user-consent="No"
        support in-subscription tickets update --ticket-name "TestTicketName" --secondary-consent [0]="{type:VirtualMachineMemoryDump,user-consent:No}"
    ```
