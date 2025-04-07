# API Reference

This page provides the OpenAPI specification that your API must implement to integrate with Tilt's platform.

You can:

- Review the required endpoints and their specifications
- Understand the expected request/response schemas
- Download the OpenAPI specification using the download button

<redoc src="openapi.yaml"></redoc>

<script>
  // Wait for the page to load
  window.addEventListener('load', function() {
    // Initialize ReDoc
    Redoc.init('openapi.yaml', {
      scrollYOffset: 60,
      hideDownloadButton: false,
      expandResponses: "200,201",
      requiredPropsFirst: true,
      noAutoAuth: true,
      pathInMiddlePanel: true,
      hideLoading: true,
      nativeScrollbars: true,
      suppressWarnings: true,
      theme: {
        colors: {
          primary: {
            main: '#3f51b5'
          }
        },
        typography: {
          fontSize: '16px',
          lineHeight: '1.5',
          fontFamily: 'Roboto, sans-serif'
        },
        sidebar: {
          width: '260px',
          backgroundColor: '#f5f5f5'
        }
      }
    }, document.getElementById('redoc-container'));
  });
</script>

<style>
  #redoc-container {
    min-height: 100vh;
    width: 100%;
  }
</style> 