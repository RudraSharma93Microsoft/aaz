# [Command] _support in-subscription tickets create_

Creates a new support ticket for Quota increase, Technical, Billing, and Subscription Management issues for the specified subscription.

## Versions

### [2022-09-01-preview](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5zdXBwb3J0L3N1cHBvcnR0aWNrZXRzL3t9/2022-09-01-preview.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/providers/microsoft.support/supporttickets/{} 2022-09-01-preview -->

#### examples

- Create a ticket for Billing related issues
    ```bash
        support in-subscription tickets create --contact-country "USA" --contact-email "abc@contoso.com" --contact-first-name "Foo" --contact-language "en-US" --contact-last-name "Bar" --contact-method "email" --contact-timezone "Pacific Standard Time" --description "BillingTicketDescription" --diagnostic-consent "Yes" --problem-classification "/providers/Microsoft.Support/services/BillingServiceNameGuid/problemClassifications/BillingProblemClassificationNameGuid" --severity "minimal" --ticket-name "BillingTestTicketName" --title "BillingTicketTitle"
    ```

- Create a ticket for Subscription Management related issues.
    ```bash
        support in-subscription tickets create --contact-country "USA" --contact-email "abc@contoso.com" --contact-first-name "Foo" --contact-language "en-US" --contact-last-name "Bar" --contact-method "email" --contact-timezone "Pacific Standard Time" --description "SubMgmtTicketDescription" --diagnostic-consent "Yes" --problem-classification "/providers/Microsoft.Support/services/SubMgmtServiceNameGuid/problemClassifications/SubMgmtProblemClassificationNameGuid" --severity "minimal" --ticket-name "SubMgmtTestTicketName" --title "SubMgmtTicketTitle"
    ```

- Create a ticket for Technical issue related to a specific resource
    ```bash
        support in-subscription tickets create --contact-country "USA" --contact-email "abc@contoso.com" --contact-first-name "Foo" --contact-language "en-US" --contact-last-name "Bar" --contact-method "email" --contact-timezone "Pacific Standard Time" --contact-additional-emails "xyz@contoso.com" "devs@contoso.com"--description "TechnicalTicketDescription" --diagnostic-consent "Yes" --problem-classification "/providers/Microsoft.Support/services/TechnicalServiceNameGuid/problemClassifications/TechnicalProblemClassificationNameGuid" --severity "minimal" --ticket-name "TechnicalTestTicketName" --title "TechnicalTicketTitle" --technical-resource "/subscriptions/SubscriptionGuid/resourceGroups/RgName/providers/Microsoft.Compute/virtualMachines/RName" --secondary-consent "[{type:VirtualMachineMemoryDump,user-consent:No}]"
    ```

- Create a ticket to request Quota increase for Compute VM Cores.
    ```bash
        support in-subscription tickets create --contact-country "USA" --contact-email "abc@contoso.com" --contact-first-name "Foo" --contact-language "en-US" --contact-last-name "Bar" --contact-method "email" --contact-timezone "Pacific Standard Time" --description "QuotaTicketDescription" --diagnostic-consent "Yes" --problem-classification "/providers/Microsoft.Support/services/QuotaServiceNameGuid/problemClassifications/CoresQuotaProblemClassificationNameGuid" --severity "minimal" --ticket-name "QuotaTestTicketName" --title "QuotaTicketTitle"  --quota-change-version "1.0" --quota-change-requests [0].region="EASTUS" --quota-change-requests [0].payload="'{\`"VMFamily\`":\`"DSv3 Series\`",\`"NewLimit\`":\`"110\`"}'"
    ```
