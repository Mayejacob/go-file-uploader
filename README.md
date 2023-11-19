# Slack File Uploader

This is a simple Go application for uploading files to Slack channels using the Slack API.

## Getting Started

### Prerequisites

- Go installed on your machine
- Slack Bot Token
- Slack Channel ID
- File(s) to upload

### Configuration

1. Create a file named `.env` in the same directory as your Go application.

2. Add the following content to the `.env` file:

    ```env
    SLACK_BOT_TOKEN=xoxb-your-bot-token
    CHANNEL_ID=your-channel-id
    ```

3. Replace `your-bot-token` and `your-channel-id` with your Slack Bot Token and Channel ID.

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Mayejacob/go-file-uploader.git
    ```

2. Navigate to the project directory:

    ```bash
    cd slack-file-uploader
    ```

3. Run the application:

    ```bash
    go run main.go
    ```

   The application will upload the specified file(s) to the Slack channel.

## Usage

Modify the `CHANNEL_ID` and `fileArr` variables in the `main.go` file to specify the target Slack channel and the file(s) you want to upload.

```go
channelArr := []string{os.Getenv("CHANNEL_ID")}
fileArr := []string{"file.pdf"}
```

## Acknowledgments

- [slack-go/slack:](https://github.com/slack-go/slack): The official Slack API library for Go.
- [joho/godotenv:](https://github.com/joho/godotenv): A Go (golang) port of the Ruby dotenv project.
- [AkhilSharma90](https://github.com/AkhilSharma90/): Acknowledging the source for inspiration.
