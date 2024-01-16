# OpenFDA Adverse Events Flutter Package

## Overview
This Flutter package provides easy and structured access to the openFDA Adverse Events API, focusing on veterinary drug reaction reports. It enables Flutter applications to query and parse adverse event data effectively.

## Features
- Easy querying of openFDA Adverse Events API.
- Automatic parsing of JSON response into Dart objects.
- Robust error handling and network request management.

## Getting Started
To use this package in your Flutter application, follow these steps:

***Installation***
Add the following dependency to your ```pubspec.yaml``` file:

```yaml
dependencies:
openfda_adverse_events_flutter: ^1.0.0
```

***Usage***
Import the package in your Dart file:

```dart
import 'package:openfda_adverse_events_flutter/openfda_adverse_events_flutter.dart';
```

Create an instance of the API service and call the methods to fetch adverse events:

```dart
OpenFDAApiService apiService = OpenFDAApiService();
String query = 'your_query_here';
apiService.fetchAdverseEvents(query: query).then((events) {
// Process events
});
```

## Documentation
For more detailed documentation regarding the API usage and models, refer to the [openFDA API documentation](https://open.fda.gov/apis/).

## Contributing
Contributions are welcome. Please read the contribution guidelines for more information.

## License
This package is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer
Do not rely on openFDA to make decisions regarding medical care. This data is not validated and is provided as-is.

