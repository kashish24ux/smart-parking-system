# smart-parking-system
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Smart Parking System</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100 text-gray-800">

  <!-- Header -->
  <header class="bg-blue-700 text-white p-6 shadow-md">
    <h1 class="text-3xl font-bold text-center">Smart Parking System</h1>
    <p class="text-center mt-2">Using ESP32-CAM for Number Plate Detection</p>
  </header>

  <!-- Hero Section -->
  <section class="p-8 text-center bg-white">
    <h2 class="text-2xl font-semibold mb-4">Welcome to Smart Parking</h2>
    <p class="max-w-xl mx-auto">Monitor vehicle entry and exit in real-time with automatic number plate detection. Designed for smart cities and efficient parking management.</p>
  </section>

  <!-- ESP32-CAM Live Feed -->
  <section class="p-8 bg-gray-50">
    <h3 class="text-xl font-semibold mb-4 text-center">Live Camera Feed</h3>
    <div class="flex justify-center">
      <!-- Replace with your ESP32-CAM stream URL -->
      <img src="http://<YOUR_ESP32_CAM_IP>:81/stream" alt="ESP32-CAM Live Feed" class="rounded-lg shadow-lg w-full max-w-3xl border">
    </div>
  </section>

  <!-- Detected Number Plates -->
  <section class="p-8 bg-white">
    <h3 class="text-xl font-semibold mb-4 text-center">Recent Detected Plates</h3>
    <div class="max-w-xl mx-auto">
      <ul id="plateList" class="bg-gray-100 rounded-lg shadow divide-y divide-gray-200">
        <!-- Example entry -->
        <li class="p-4">ABC123 - 2025-04-05 10:32 AM</li>
        <li class="p-4">XYZ987 - 2025-04-05 10:29 AM</li>
        <!-- Populate with JS + Firebase -->
      </ul>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-blue-700 text-white p-6 mt-8">
    <p class="text-center">&copy; 2025 Smart Parking System. All rights reserved.</p>
  </footer>

  <!-- Firebase integration script (example placeholder) -->
  <script type="module">
    // TODO: Replace with your Firebase config and logic to fetch recent plate numbers
    // Example: fetch from Firestore and populate #plateList
  </script>

</body>
</html>