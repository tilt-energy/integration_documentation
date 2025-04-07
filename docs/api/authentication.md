# Authentication

## OAuth2 Authentication

Your API must implement [OAuth2](https://en.wikipedia.org/wiki/OAuth) with client credentials flow for authentication. Tilt will use this to authenticate with your system:

### Authentication Flow

1. Tilt will provide client credentials (client ID and secret)
2. Tilt will request an access token using your `/oauth/token` endpoint
3. Tilt will use the access token in the `Authorization` header for subsequent requests
4. The token should expire after a set period

### Required Headers

```http
Authorization: Bearer <access_token>
```

## Secret Sharing

To ensure secure communication, certain sensitive information must be shared securely:

1. Create a text file containing your secrets
2. Encrypt the file using our public PGP key:
   - Key ID: `FFCFBF1B68B2EDE1B6228D8BF4F186FED63ED956`
   - Available on [keys.openpgp.org](https://keys.openpgp.org/search?q=integration-support%40tilt-energy.com)
The verified owner of this key should be Tilt Integration Support<integration-support@tilt-energy.com>
3. Send the encrypted file to: integration-support@tilt-energy.com