# Countries Info Application

A simple front-end application that fetches and displays information about countries using the public REST Countries API. It includes two implementations (V1 and V2) to illustrate incremental improvements in HTML/CSS/JavaScript usage and UI/UX.

> Note: The legacy endpoint https://restcountries.eu/ has been retired. The current API is available at https://restcountries.com/. If you experience issues fetching data, update the endpoint in your code to use the new domain and paths (see API section below).

## Features
- Search and explore countries
- View key details: flag, name, capital, region, population, currencies, languages, and more
- Client-side rendering with AJAX requests
- Two versions (V1 and V2) to compare structure and styling approaches

## Project structure
```
.
├─ README.md
└─ countries/
   ├─ CountriesV1/
   │  ├─ countries.html
   │  └─ countries.css
   └─ CountriesV2/
      ├─ countries.html
      ├─ countriesjs.js
      └─ countriesstyle.css
```

## Getting started
You can run this project as a static website. No build tools are required.

- Option A: Open directly
  1. Navigate to the folder on your machine.
  2. Double-click one of the HTML files:
     - countries/CountriesV1/countries.html
     - countries/CountriesV2/countries.html

- Option B: Serve locally (recommended for consistent AJAX behavior)
  - Using PowerShell (Windows 10+):
    - Python: `python -m http.server 8080` (serve current directory) and open http://localhost:8080/
    - Node: `npx serve -p 8080` (if you have Node.js) and open http://localhost:8080/

## Usage
- Open V1 or V2 HTML in a browser.
- Interact with the UI to search or browse countries.
- Country data will be fetched via AJAX and rendered on the page.

## API
- Original (deprecated): https://restcountries.eu/
- Current: https://restcountries.com/

Common endpoints on the new API (v3.1):
- All countries: https://restcountries.com/v3.1/all
- By name: https://restcountries.com/v3.1/name/{name}
- By region: https://restcountries.com/v3.1/region/{region}

The response shape in v3.1 differs from the old API (e.g., nested objects for names, currencies, and languages). If you migrate the endpoint, be prepared to adjust property paths in JavaScript accordingly.

## Technologies used
* HTML5 		![](https://img.shields.io/badge/Code-HTML5-informational?style=flat&logo=html5)
* CSS3			![](https://img.shields.io/badge/Code-CSS3-informational?style=flat&logo=CSS3)
* JavaScript	![](https://img.shields.io/badge/Code-JavaScript-informational?style=flat&logo=javascript)
* jQuery		![](https://img.shields.io/badge/Library-jQuery-informational?style=flat&logo=jquery)
* AJAX

## Screenshots
You can add screenshots or GIFs here to showcase the UI.
- V1: [Add screenshot]
- V2: [Add screenshot]

## Browser support
- Modern desktop and mobile browsers. No specific polyfills are included.

## Accessibility
- Basic semantic HTML. Additional improvements are welcome.

## Contributing
Contributions, issues, and feature requests are welcome.
- Fork the repository
- Create a feature branch: `git checkout -b feat/your-feature`
- Commit your changes: `git commit -m "feat: add your feature"`
- Push to the branch: `git push origin feat/your-feature`
- Open a Pull Request

## License
No explicit license file is included at this time. If you plan to reuse or distribute this code, consider adding a license that fits your needs (e.g., MIT, Apache-2.0).

## Acknowledgments
- REST Countries (https://restcountries.com/) for the public dataset and API.
