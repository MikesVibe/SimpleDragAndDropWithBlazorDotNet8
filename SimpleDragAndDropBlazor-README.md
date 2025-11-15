# Simple Drag and Drop with Blazor .NET 8

An example of simple drag and drop with Blazor, now supporting both **Server** and **WebAssembly** interactive render modes.

## Features

This application demonstrates:
- Drag and drop functionality with Blazor components
- **Server-side rendering** with SignalR for real-time interactivity
- **WebAssembly rendering** for client-side execution
- Shared components and models between both render modes
- Easy navigation between Server and WebAssembly modes

## Project Structure

- **SimpleDragAndDropBlazorApp** - The main server project that hosts the application
  - Contains shared components (`Components/Shared/`)
  - Contains models (`Models/`)
  - Serves pages with both Server and WebAssembly render modes
- **SimpleDragAndDropBlazorApp.Client** - The WebAssembly client project
  - Contains client-specific code and pages

## Running the Application

1. Navigate to the `SimpleDragAndDropBlazorApp` directory:
   ```bash
   cd SimpleDragAndDropBlazorApp/SimpleDragAndDropBlazorApp
   ```

2. Run the application:
   ```bash
   dotnet run
   ```

3. Open your browser and navigate to the displayed URL (typically `https://localhost:5xxx`)

## Using the Application

The application features two modes accessible via the navigation menu:

- **Server Mode** (`/`) - Uses Interactive Server rendering, executing code on the server with SignalR communication
- **WebAssembly Mode** (`/wasm`) - Uses Interactive WebAssembly rendering, executing code in the browser

Both modes demonstrate the same drag and drop functionality:
1. Drag tasks between the three columns: Todo, Started, and Completed
2. See real-time updates to task status
3. View the last updated task information

## Screenshots

### Server Mode
![Server Mode](https://github.com/user-attachments/assets/eb52af1d-9065-4b96-a6f3-f89e0f8ec8d6)

### WebAssembly Mode
![WebAssembly Mode](https://github.com/user-attachments/assets/1765e9d1-d5fa-414b-83aa-8f70b1a1019e)

## Original Blog Post

Read the full blog post at [https://chrissainty.com/investigating-drag-and-drop-with-blazor/](https://chrissainty.com/investigating-drag-and-drop-with-blazor/).

## Technology Stack

- .NET 8
- Blazor Server
- Blazor WebAssembly
- Interactive render modes
