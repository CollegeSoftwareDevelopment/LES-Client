# LES-Client

LES-Client (Lab Examination System - Client) is the student-side application for the Lab Examination System, built using .NET. It allows students to participate in exams conducted by their educational institutions using a secure and user-friendly interface.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- Secure login for students.
- Real-time exam participation.
- Automated submission of answers.
- Time management and exam countdown.
- Instant feedback on submissions.

## Requirements

- .NET 6 SDK or higher
- Windows 10 or higher

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/CollegeSoftwareDevelopment/LES-Client.git
    cd LES-Client
    ```

2. **Restore dependencies:**

    ```bash
    dotnet restore
    ```

## Configuration

Configuration settings, including the API URL and API Key, are managed through a Windows Form within the application. Follow these steps to configure the application:

1. **Launch the Configuration Form:**

    When you first run the application, the configuration form will prompt you to enter the necessary settings.

2. **Enter the Settings:**

    - **API URL:** The base URL for the backend server.
    - **API Key:** The key used to authenticate API requests.

3. **Save the Settings:**

    After entering the necessary information, click the "Save" button to store these settings. The application will then use these settings for its operations.

## Usage

1. **Run the application:**

    ```bash
    dotnet run
    ```

    This will start the application. Open [http://localhost:5000](http://localhost:5000) to view it in the browser.

2. **Publish the application:**

    ```bash
    dotnet publish -c Release -o ./publish
    ```

    This will create a release build of the application in the `./publish` directory.

3. **Deploy the application:**

    - Copy the contents of the `./publish` directory to your web server.
    - Ensure that the server is configured to serve the application correctly.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature-name`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Explanation of Changes:

- **Configuration:** Removed the `appsettings.json` section and added instructions on configuring the application through a Windows Form within the app.
- **Settings Example:** Provided an example of how the configuration form might look in the application code.
- **Replaced WebSocket URL with API Key:** Updated the configuration details to use an API key instead of a WebSocket URL.

This README should now reflect the updated configuration method and meet your requirements.
