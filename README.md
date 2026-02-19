# MapAccess

An iOS demo app showcasing MapKit fundamentals using SwiftUI's native `Map` view.

## Features

- **User Location Tracking** — `CLLocationManager` integration with permission handling, live location display, and center-on-user control
- **Annotations & Callouts** — Custom map markers with tappable callouts displaying point-of-interest details
- **Local Search** — `MKLocalSearch` to find nearby points of interest and display results as map annotations
- **Map Style Toggle** — Switch between standard, satellite, and hybrid views

## Architecture

| File | Purpose |
|------|---------|
| `LocationService.swift` | `ObservableObject` wrapping `CLLocationManager` — authorization, location tracking, error handling |
| `MapSearchService.swift` | `MKLocalSearch` wrapper — POI search, result management |
| `MapAnnotationModel.swift` | Data model for map annotations |
| `ContentView.swift` | SwiftUI interface composing the map, search bar, and controls |

## Requirements

- iOS 17+
- Xcode 15+
- Physical device recommended (simulator supports simulated location)

## Setup

1. Clone the repository
2. Open `MapAccess.xcodeproj` in Xcode
3. Build and run on a device or simulator
4. Allow location access when prompted
