# DataStax + Vercel AI SDK 3.0 Generative UI demo

This is a demo of an interactive financial assistant. It can show you stocks, tell you their prices, and even help you buy shares. 

Check out our [blog post](https://datastax.com/blog) for a more detailed breakdown of the codebase and how this app works.

## Getting Started

### Prerequisites

- An Astra DB account. You can [create one here](https://astra.datastax.com/signup).
    - An Astra Vector Database
- An OpenAI account and api key [create one here](https://platform.openai.com/)

### Setup

1. Clone this repository to your local machine.
2. Install the dependencies by running `npm install` in your terminal.
3. Set up the following environment variables in your IDE or `.env` file:
    - `OPENAI_API_KEY`: api key for OPENAI
    - `ASTRA_DB_ENDPOINT`: Your Astra DB vector database endpoint
        - Copy from the `Database Detail`
    - `ASTRA_DB_APPLICATION_TOKEN`: The generated app token for your Astra database
        - To create a new token go to your database's `Connect` tab and click `Generate Token`. (your Application Token begins with `AstraCS:...`)
4. Create a collection (vector disabled) and load the `data/sp500_companies.csv` data into it

### Running the Project

To start the development server, run `npm run dev` in your terminal. Open [http://localhost:3000](http://localhost:3000) to view the chatbot in your browser.