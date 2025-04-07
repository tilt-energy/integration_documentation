# API Overview

This section describes the API specification that your system must implement to integrate with Tilt's platform. Your API must conform to this specification to ensure successful integration.

## Authentication

Your API must implement OAuth2 with client credentials flow for authentication. Tilt will use this to authenticate with your system:

1. Tilt will provide client credentials (client ID and secret)
2. Tilt will request an access token using your `/oauth/token` endpoint
3. Tilt will use the access token in the `Authorization` header for subsequent requests

## Documentation

For detailed API specification, including:

- Required endpoints and their specifications
- Expected request/response schemas
- Authentication requirements

Please visit our [API Reference](reference.md) page. 