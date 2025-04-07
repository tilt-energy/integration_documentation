# Integration Validation Process

This page describes the validation process that third-party developers should follow to ensure their implementation meets Tilt's requirements and can be successfully integrated.

## Step 1: Specification Review

Before starting the validation process, review your implementation against this specification. If you identify any divergences:

1. Document the differences between your implementation and this specification
2. Document your data specificities (error cases, device types, field names...)
3. Contact the Tilt integration team at [integration-support@tilt-energy.com](mailto:integration-support@tilt-energy.com) to discuss these divergences
4. We will work together to determine if these differences are acceptable or if adjustments are needed

## Step 2: Test Environment Setup

To begin the validation process, you need to provide:

1. A test environment ("preprod" or "staging") that mirrors your production environment
2. Credentials for Tilt to connect to your test environment
3. Any specific configuration or setup instructions needed to access your test environment
4. A description of any meaningful limitation or difference between your test and production environments, including:
    - Performance limitations
    - Availability and maintenance windows
    - Dataset inconsistencies
    - Any other relevant constraints

Send these details to [integration-support@tilt-energy.com](mailto:integration-support@tilt-energy.com).

## Step 3: Integration Testing

Once we have access to your test environment:

1. Tilt will adapt our standard integration test suite to your specific implementation
2. We will validate both technical and functional requirements
3. We will provide feedback and work with you to address any issues found

Ready to move forward? Congratulations! Let's begin the [Tilt Integration phase](tilt_integration.md) to connect your implementation with our platform.
