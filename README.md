
Welcome to TeckPhoto, a feature-rich, progressive web application (PWA) that allows you to upload or capture photos, view them in a gallery, see their locations on a map, and export location data.

This application is built with modern web technologies including:

- **Next.js** (App Router)
- **React** & **TypeScript**
- **Tailwind CSS** for styling
- **Shadcn/UI** for beautiful, accessible components
- **@vis.gl/react-google-maps** for Google Maps integration
- **PWA support** for an installable, app-like experience on mobile devices.

## Features

- **Dual Photo Input**: Upload photos from your device or capture them directly using your camera.
- **Metadata Simulation**: Automatically generates date, time, and geolocation for each photo.
- **Interactive Gallery**: View your photos in a responsive grid.
- **Map View**: See markers for each photo on an interactive Google Map.
- **Photo Details**: Click on any photo to see a larger view, its description, and metadata.
- **Data Export**: Download geolocations as a KML file for use in Google Earth or as an SQL file for database import.
- **Multi-language**: Supports English and Spanish.
- **Theming**: Switch between light and dark modes.

## Getting Started

Follow these instructions to get the project up and running on your local machine.

### Prerequisites

- Node.js (v18 or later)
- npm, yarn, or pnpm
- A Google Maps API Key

### Installation

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd TeckPhoto
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Set up your environment variables:**
    Create a file named `.env.local` in the root of your project and add your Google Maps API key:
    ```
    NEXT_PUBLIC_GOOGLE_MAPS_API_KEY=YOUR_API_KEY_HERE
    ```
    You can obtain a key from the [Google Cloud Console](https://console.cloud.google.com/google/maps-apis/overview). Make sure to enable the "Maps JavaScript API".

### Running the Development Server

Once the dependencies are installed, you can start the development server:

```bash
npm run dev
```

Open [http://localhost:9002](http://localhost:9002) with your browser to see the result.

## Project Structure

- `src/app/`: Contains the main application pages and layouts.
- `src/components/`: Contains reusable React components.
- `src/components/ui/`: Contains the Shadcn/UI components.
- `src/types/`: Contains TypeScript type definitions.
- `public/`: Contains static assets like icons and the manifest file.
