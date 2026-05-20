# How Copilot accesses data using Microsoft Graph and Permissions

## Links

- [Microsoft](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/overview-copilot-connector)

## Notes

- Prompt flow
  - All activities are in Microsoft 365 service boundary
    - User sends prompt to Copilot using Microsoft app or chat
    - Prompt is preprocessed or grounded using data in Microsoft 365 tenant
      - Accessed using the Microsoft Graph
      - Data is encrypted in transit and at rest
    - Copilot sends grounded data to LMM/Azure OpenAI service
    - LLM returns data back to Copilot
    - Copilot returns data to user
    - Data is not used to train LLMs
  