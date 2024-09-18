
# Botpress Demo Project

This repository contains the code for a chatbot built using **Botpress SDK**. The bot is designed with customizable Q&A functionality and will eventually support multi-language responses and API integration.

## Features
- **Customizable Q&A Bot**: The bot answers predefined questions and can be easily expanded.
- **Multi-language Support**: (To be implemented)
- **External API Integration**: (To be implemented)
- **User-friendly Interface**: Provides smooth interactions and feedback.

## Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/maddydevgits/botpress-demo-project.git
   cd botpress-demo-project
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run the Botpress SDK server:**
   ```bash
   npm start
   ```

4. **Access the bot interface:**
   Open your browser and navigate to `http://localhost:3000`.

## Usage

- The bot is pre-configured with a basic Q&A flow. You can test the bot by asking common questions like "What is your name?" or "Hello."
  
  Example Q&A interaction:
  - **User**: "Hello"
  - **Bot**: "Hello! How can I assist you today?"

- The bot will provide fallback responses for unrecognized queries.

## Adding Custom Questions

To add more Q&A responses:
1. Open `qa.js`.
2. Add new patterns and corresponding answers. For example:
   ```javascript
   bp.hear(/what is the weather/i, (event, next) => {
     event.reply('#builtin_text', { text: 'The weather is great today!' })
   })
   ```

## Roadmap

- **Multi-language support**: We will implement language detection and responses in various languages.
- **API Integration**: Add API-based responses for dynamic content (e.g., weather, news).

## Contributing

Feel free to fork this repository and contribute. Submit a pull request with improvements or new features.

## License

This project is licensed under the MIT License.
