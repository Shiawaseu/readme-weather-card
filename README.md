## Generate and embed beautiful, themeable weather cards with Github Actions

<p align="center">
  <img src="https://raw.githubusercontent.com/Shiawaseu/readme-weather-card/main/public/cards/weather-dark.png" alt="Weather Card" width="510" height="300"/>
</p>

## Features

- ✅ GitHub-compatible, exported as `PNG/GIF` image output
- 🎨 Multiple theme support, with easy configuration
- ⚡ Fast preview while designing with `Fastify`
- ⚒️ Builds with `Github Actions`, and updates every 30 minutes!


---

## 🖼️ Example Themes

<details>
  <summary>Click here to preview themes</summary>
  <br/>
  <table>
    <thead>
      <tr>
        <th>Theme</th>
        <th>Preview</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Dark (Default)</td>
        <td><img src="https://raw.githubusercontent.com/Shiawaseu/readme-weather-card/main/public/cards/weather-dark.png" alt="Dark theme" /></td>
      </tr>
      <tr>
        <td>Light</td>
        <td><img src="https://raw.githubusercontent.com/Shiawaseu/readme-weather-card/main/public/cards/weather-light.png" alt="Light theme" /></td>
      </tr>
      <tr>
        <td>Plurple</td>
        <td><img src="https://raw.githubusercontent.com/Shiawaseu/readme-weather-card/main/public/cards/weather-plurple.png" alt="Plurple theme" /></td>
      </tr>
      <tr>
        <td>GitHub-dark</td>
        <td><img src="https://raw.githubusercontent.com/Shiawaseu/readme-weather-card/main/public/cards/weather-github-dark.png" alt="GitHub-dark theme" /></td>
      </tr>
      <tr>
        <td>GitHub-light</td>
        <td><img src="https://raw.githubusercontent.com/Shiawaseu/readme-weather-card/main/public/cards/weather-github-light.png" alt="GitHub-light theme" /></td>
      </tr>
    </tbody>
  </table>
</details>



---

## ❓ Usage

<details>
  <summary>Click to show installation instructions</summary>
  <ol>
    <li>Clone or fork this repository</li>
    <li>Edit <code>/configuration/config.json</code> to match your city:
      <ul>
        <li>For city IDs, visit <a href="http://bulk.openweathermap.org/sample/">this page</a> or use the <a href="https://openweathermap.org/find">search tool</a> and copy the ID from the URL</li>
        <li>Longitude and latitude are <strong>optional</strong> but improve accuracy</li>
      </ul>
    </li>
    <li>Register at <a href="https://openweathermap.org/">OpenWeather</a> and create your API key <a href="https://home.openweathermap.org/api_keys">here</a></li>
    <li>Go to your GitHub repo's <strong>Settings &gt; Secrets and variables &gt; Actions &gt; Repository secrets</strong> and add:
      <ul>
        <li><code>OPENWEATHER_API_KEY</code> with your API key as the value</li>
      </ul>
    </li>
    <li>You're done! Optionally, add a new theme file to <code>/configuration/themes</code>:
      <ul>
        <li>Note: more themes = more compile time in the GitHub Actions workflow</li>
      </ul>
    </li>
        <li>Go and visit your <code>actions</code> page to enable the workflow
      <ul>
        <li>You'll have to manually re-enable the workflow the first time</li>
      </ul>
    </li>
  </ol>
</details>
