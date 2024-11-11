Summary of the document:

The content provided is a Terraform resource documentation for managing an Azure Active Directory B2C (AAD B2C) Directory using the `azurerm_aadb2c_directory` resource. Here is a summary of the key points:

### Resource Overview
- **Purpose**: Manages an AAD B2C Directory.
- **Example Usage**: An example configuration is provided, showing how to create an AAD B2C Directory with specific settings:
  ```hcl
  resource "azurerm_aadb2c_directory" "example" {
    country_code            = "US"
    data_residency_location = "United States"
    display_name            = "example-b2c-tenant"
    domain_name             = "exampleb2ctenant.onmicrosoft.com"
    resource_group_name     = "example-rg"
    sku_name                = "PremiumP1"
  }
  ```

### Arguments Reference
- **Arguments**:
  - **`country_code`**: Optional; Country code of the B2C tenant. Required when creating a new resource.
  - **`data_residency_location`**: Required; Location where the B2C tenant is hosted and data resides. Possible values are `Asia Pacific`, `Australia`, `Europe`, `Global`, and `United States`.
  - **`display_name`**: Optional; Initial display name of the B2C tenant. Required when creating a new resource.
  - **`domain_name`**: Required; Domain name of the B2C tenant, including the `.onmicrosoft.com` suffix.
  - **`resource_group_name`**: Required; Name of the Resource Group where the AAD B2C Directory should exist.
  - **`sku_name`**: Required; Billing SKU for the B2C tenant. Must be one of `PremiumP1` or `PremiumP2`. Standard is not supported.
  - **`tags`**: Optional; Mapping of tags to be assigned to the AAD B2C Directory.

### Attributes Reference
- **Attributes**:
  - **`id`**: The ID of the AAD B2C Directory.
  - **`billing_type`**: The type of billing for the AAD B2C tenant. Possible values include `MAU` or `Auths`.
  - **`effective_start_date`**: The date from which the billing type took effect. May not be populated until after the first billing cycle.
  - **`tenant_id`**: The Tenant ID for the AAD B2C tenant.

### Timeouts
- The `timeouts` block allows specifying timeouts for certain actions:
  - **`create`**: Defaults to 30 minutes.
  - **`read`**: Defaults to 5 minutes.
  - **`update`**: Defaults to 30 minutes.
  - **`delete`**: Defaults to 30 minutes.

### Import
- AAD B2C Directories can be imported using the resource ID:
  ```shell
  terraform import azurerm_aadb2c_directory.example /subscriptions/12345678-1234-9876-4563-123456789012/resourceGroups/example-resource-group/providers/Microsoft.AzureActiveDirectory/b2cDirectories/directory-name
  ```
