# LocationApp

LocationApp is a simple Android application that allows users to retrieve and display their current location information.

## Features

- Get real-time latitude and longitude coordinates
- Reverse geocode location to obtain address information
- Request location permissions dynamically
- Utilizes the Fused Location Provider for accurate location updates

## Screenshots

<figure>
    <img src="https://github.com/pavan-kumar-arepu/LocationnApp/assets/13812858/f503c800-255e-47a1-89c0-53eff44519bf" alt="Initial-GetLocation" style="width:45%;">
    <img src="https://github.com/pavan-kumar-arepu/LocationnApp/assets/13812858/81440368-faa7-44c8-9148-3bd357056c20" alt="LocationNotAvailable" style="width:45%; margin-right: 10px;">
    <img src="https://github.com/pavan-kumar-arepu/LocationnApp/assets/13812858/b53d210a-896c-4ca3-8c67-52cd73f36efc" alt="When User Denied Access" style="width:45%; margin-right: 10px;">
 <img src="https://github.com/pavan-kumar-arepu/LocationnApp/assets/13812858/7757ba73-7ad2-483a-8c95-19ed32fec444" alt="Latitude and Longitude" style="width:45%; margin-right: 10px;">
</figure>


## Architecture

The LocationApp follows a clean architecture design, separating the application into layers for better maintainability and testability.

### Layers

1. **Presentation Layer**
   - **MainActivity:** Entry point of the app. Responsible for setting up the UI and interacting with the ViewModel.
   - **MyApp Composable:** Composable function for UI setup using Jetpack Compose.
   - **LocationDisplay Composable:** Composable function for displaying location details and handling location updates.

2. **ViewModel**
   - **LocationViewModel:** Manages the app's location-related data and communicates with the UI.

3. **Domain Layer**
   - **LocationData:** Data class representing latitude and longitude coordinates.

4. **Data Layer**
   - **LocationUtils:** Utility class for handling location-related tasks, including requesting updates and reverse geocoding.
  
## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/LocationApp.git

2. Open the project in Android Studio.
3. Build and run the app on your emulator or physical device.

## Permissions
The app requires the following permissions:

Fine Location (ACCESS_FINE_LOCATION)
Coarse Location (ACCESS_COARSE_LOCATION)
Ensure that these permissions are granted for the app to function correctly.

## Contributions
Contributions are welcome! Feel free to open issues or submit pull requests.
