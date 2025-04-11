# Document Your System

This page outlines the essential documentation you need to provide about your API implementation. Clear documentation of your data structures and behaviors is crucial for successful integration with Tilt's platform.

## Required API Documentation

### 1. Device Types & tags
Document all device types that your system supports and how we should control them, as well
as the device tags.

Ex : An HVAC should be stopped by writing HEATING-MODE to FROST-PROTECTION, unless it has a tag "HITASHI", in which case its TEMPERATURE-TARGET should be set to 16°C.

### 2. Error Cases
Document all foreseeable error scenarii:

```yaml
errors:
  - error_key: "field_not_writable"
    description: "Attempted to write to a read-only field"
    error_details:
      field_name: "FEEDBACK-SENSOR"
  
  - error_key: "device_not_found"
    description: "Requested device does not exist"
    error_details:
      device_id: "550e8400-e29b-41d4-a716-446655440001"
  
  - error_key: "value_out_of_bounds"
    description: "Provided value is invalid for the field"
    error_details:
      field_name: "TEMPERATURE-TARGET"
      provided_value: 41
      min: 5
      max: 30
```

## Documentation Requirements

1. **Completeness**
    - Document all device types and their capabilities
    - Include all possible error scenarios

2. **Clarity**
    - Provide clear descriptions for each element
    - Include examples where helpful
    - Specify units and constraints

3. **Accuracy**
    - Keep documentation up-to-date with your implementation
    - Document any limitations or special cases
    - Include version information if applicable

## Need Help?

If you need assistance with documenting your data, please contact our integration team at [integration-support@tilt-energy.com](mailto:integration-support@tilt-energy.com).