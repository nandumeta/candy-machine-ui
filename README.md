## Candy Machine User Interface: Step-by-Step Guide

This guide walks you through setting up the user interface (UI) for your Candy Machine. Users will be able to mint NFTs using your custom SPL token through their Phantom wallets.

**Before you begin:**

* **Ensure your Candy Machine is configured:** Your `config.json` file should define details like price, quantity, token symbol, fees, SPL token information (account & address), go-live date, and creator details.
* **Have a Phantom wallet:** This is what users will connect to mint NFTs.
* **Create a new SPL token:** Make sure you follow the instructions from Lesson Three and note down the token address.

**Steps:**

1. **Set up your SPL Token:**
   * If you haven't already, follow the instructions from Lesson Three to create an SPL token. Remember the token's address.

2. **Update Candy Machine Configuration:**
   * Edit your Candy Machine's `config.json` file and update the following fields:
     * `splTokenAccount`: Replace with the address of your created SPL token account.
     * `splToken`: Replace with the address of your newly created SPL token.

3. **Configure the User Interface (UI):**
   * Refer to the "Quick Node: Set Up a Minting Site" tutorial (link not provided) to learn how to create a UI for your Candy Machine. This UI should allow users to connect their Phantom wallets and mint NFTs using the SPL token for payment.

4. **Adjust Minting Logic:**
   * Modify the minting logic within your SPL project (refer to Lesson Three) to:
     * Mint NFTs directly to the user's Phantom wallet address.
   * Alternatively, adapt the transfer function to deliver minted NFTs to your designated Phantom wallet.

5. **Testing:**
   * Test the entire setup thoroughly. 
     * Transfer or mint your SPL token to a test Phantom account.
     * Use the UI to mint NFTs, ensuring users can seamlessly pay with the designated SPL token.

