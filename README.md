<body>

<h1>LED Status Controller with ESP8266</h1>

<p>This project uses an ESP8266 microcontroller to control four LEDs or anything else you want based on data received from a REST API.</p>

<h2>Setup</h2>

<ol>
    <li>
        <strong>Hardware Connections:</strong>
        <ul>
            <li>Connect four LEDs to the ESP8266 pins:</li>
            <ul>
                <li>LED 1: GPIO D0</li>
                <li>LED 2: GPIO D1</li>
                <li>LED 3: GPIO D2</li>
                <li>LED 4: GPIO D3</li>
            </ul>
        </ul>
    </li>
  <li></li>
    <li>
        <strong>Wi-Fi Configuration:</strong>
        <p>Set your Wi-Fi credentials in the code:</p>
        <pre>
        <code>
        const char* ssid = "your-SSID";
        const char* password = "your-password";
        </code>
        </pre>
    </li>
 <li></li>
    <li>
        <strong>API URL:</strong>
        <p>Set the API endpoint URL in the code:</p>
        <pre><code>String API_URL_GET = "https://your-api-url/endpoint";
        </code></pre>
    </li>
</ol>

<h2>How It Works</h2>
<ul>
    <li>The ESP8266 connects to your Wi-Fi network.</li>
    <li>It sends an HTTPS GET request to the API.</li>
    <li>The API returns the LED statuses in JSON format.</li>
    <li>The ESP8266 sets the LED pins based on the response.</li>
</ul>

<h2>Usage</h2>
<p>Upload the code to the ESP8266 using the Arduino IDE. The LEDs will turn on or off according to the data received from the API.</p>

<p>This project demonstrates a simple way to control hardware with data from the web using an ESP8266.</p>

<p>Enjoy The Process</p>

</body>
</html>
