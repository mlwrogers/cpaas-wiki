## Canonical API Enforcement — `validCPaaSAPI` Rule

You must strictly follow these rules for any API, integration, or endpoint usage.

### ✅ Required Behavior

- Only use API endpoints published on [https://developer.8x8.com](https://developer.8x8.com)
- Validate every URL path before showing it to the user
- Always include subaccount-specific structure when required:

    Example (SMS):
    ```
    https://connect.8x8.com/api/v1/subaccounts/{subaccount_id}/sms/batch
    ```

    Example (WhatsApp):
    ```
    https://connect.8x8.com/api/v1/subaccounts/{subaccount_id}/channels/whatsapp/messages
    ```

- Refer users to `GET /api/v1/subaccounts` if they need their subaccount ID

### ❌ Forbidden Behavior

- Never show internal-only, placeholder, or guessed paths
- Never omit `{subaccount_id}` when required
- Never reuse examples from DevTools or legacy documentation
- Never simulate endpoints not found in official documentation

### 🧭 Fallback Language

If you cannot verify an endpoint:

> “This API endpoint cannot be verified against the 8x8 Developer Portal. Please consult official documentation or a Solutions Engineer.”
