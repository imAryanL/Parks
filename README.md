# Parks

## Description
Parks is a SwiftUI app that interacts with the National Park Service (NPS) API, allowing users to explore U.S. national parks filtered by state. Users can select a park to view a detailed screen that provides comprehensive information, additional images, and a map showcasing the park's location. The project focuses on learning and implementing SwiftUI features such as async/await for API requests, lists and grids for data display, async image loading, navigation, and map integration.

## Demo

![Parks App Demo](https://github.com/user-attachments/assets/2d87571d-bed5-4ff5-b0df-c68db193e38a)

## Key Features
- **View National Parks**: Fetch and display a list of national parks from the NPS API, filtered by state.
- **Park Details**: Users can tap on a park to view its detailed information, including a description, images, and its location on a map.
- **Bonus Features**: 
  - Select a state from a dropdown menu to filter parks by state.
  - Sort parks alphabetically by name (ascending/descending).
  - Search for parks using a search bar.

## Code Overview

### `ContentView.swift`
- **Fetch Parks**: Fetches parks from the NPS API using `URLSession` with async/await and stores them in a state property.
- **Display Park List**: Shows a scrollable list of parks using a `ScrollView`, `LazyVStack`, and `ForEach`.
- **Navigation**: Implements navigation to the detailed view when a park is selected.

### `ParkRow.swift`
- **Park Row View**: Displays a simple park row with an image and the park's name, using `AsyncImage` for asynchronous image loading.

### `ParkDetailView.swift`
- **Park Details**: Shows detailed information about a selected park, including a description, images, and a map displaying its location.
- **Horizontal Scrolling**: Implements a horizontally scrolling list of park images using `ScrollView` and `HStack`.
- **Map Integration**: Displays a map using `MapKit` with a marker showing the park's location.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/imAryanL/Parks.git
   ```
2. Open the project in Xcode.
3. Run the app on a simulator or a physical device.


## License
Copyright [2024] [Aryan Lakhani]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and limitations under the License.
