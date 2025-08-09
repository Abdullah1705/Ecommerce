
#  AI-Powered Product Catalog with Smart Search (NLP)

This is a React-based e-commerce product catalog with an **AI-powered Smart Product Search** feature.  
Using **Natural Language Processing (NLP)**, users can search with phrases like:  
> "Show me running shoes under $100 with good reviews"

---

## 🚀 How to Run the App

1. **Clone the repository**
   ```bash
    git clone https://dredsoftlabs-admin@bitbucket.org/dredsoftlabs/ecommerce.git
   cd eCommerce
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Setup Environment Variables**

   * Create a `.env` file in the root directory.
   * Copy contents from `.env.example`.
   * Replace `your_api_key_here` with your **actual OpenAI API key**.
   * Example:

     ```env
     OPENAI_API_KEY=your_api_key_here
     ```

4. **Run the app**

   ```bash
   npm start
   ```

---

## 🧠 AI Feature Used

**Smart Product Search (NLP)**
We use a basic NLP library (`compromise`) to extract user intent from natural language queries, such as filtering by price, category, and review quality.
Optionally, this can be enhanced using the **OpenAI API** for more advanced language understanding.

---

## 🛠 Tools & Libraries Used (NLP Related)

* [`compromise`](https://github.com/spencermountain/compromise) — lightweight NLP library for extracting keywords and numbers from text.
* **OpenAI API (optional)** — for advanced semantic understanding and context-aware search (requires `OPENAI_API_KEY`).

---
**BONUS:**
I can connect the AI search with blockchain so that some product filters or discounts only unlock if the user holds a certain crypto token (token-gated pricing).
The AI could also read a user’s on-chain shopping preferences (stored in a wallet or smart contract) to give more personal product results.
For loyalty, every purchase could trigger a smart contract that rewards tokens, and the AI could use those tokens to suggest special offers or early access.

I can do this by:

* Checking the user’s wallet with a Web3 library (like `ethers.js`) before showing prices.
* Reading/writing preference data to a smart contract on a blockchain.
* Linking the AI’s search filters with these blockchain data checks.

```
