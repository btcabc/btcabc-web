---
layout: post
title:  "How To Start Accepting Lightning Payments: A Step-by-Step Guide"
date:   2024-08-09 18:13:48 +0100
categories: how-to 
---
Accepting Bitcoin via Lightning paymets isn't as difficult as it might sound. One can opt for a fully managed solution like [Lightspark](https://www.lightspark.com/) or run their own Lightning node and payment processor ([BTCPay Server](https://btcpayserver.org/)). This second option has now become much easier thanks to solutions like [Voltage](https://voltage.cloud/).

The steps below will guide you through setting up a Lightning Payments system with Voltage, enabling you to receive payments efficiently for your business. The tutorial covers creating a Voltage account, setting up a Lightning node, and integrating with BTC Pay Server.

You can follow the steps below or see a full tutorial in this Youtube video:

<iframe width="560" height="315" src="https://www.youtube.com/embed/7v5iQQ3g1X4?si=2H-dNIpGyrVcfWzw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Step 1: Create a Voltage Account

1. **Visit Voltage**: Go to [Voltage.cloud](https://voltage.cloud).
2. **Sign Up**:
   - Click on the "Sign Up" button in the upper right corner.
   - Enter your email and a password of your choice, then click "Register."
   - Verify your email by entering the code sent to your inbox.

3. **Log In**: Use your registered email and password to log into your Voltage account.

## Step 2: Set Up Your Lightning Node

1. **Create a Node**:
   - Click on "Create Node" and select "Lightning Node."
   - Choose the standard plan and select “mainnet,” then click "Continue."

2. **Node Configuration**:
   - Give your Lightning node a unique name (this will be public).
   - Set a different password for your node (different from your Voltage account password).
   - Click "Create" and wait for the node to start.

3. **Open a Free Channel**: 
   - You will be prompted to accept a free channel of 500,000 satoshis for liquidity.
   - Click "Accept" and wait for the channel to open (this can take some time due to on-chain confirmations).

## Step 3: Generate LNC Pairing Phrase

1. **Access the Terminal**:
   - Click on “Terminal Web” and log in using your node password.

2. **Create LNC Pairing Phrase**:
   - Name your connection and select "Admin Macaroon" type.
   - Click “Create LNC Pairing Phrase” and copy it.
   
3. **Launch Terminal**: 
   - Go to `terminal.lightning.engineering` and click "Connect My Node."
   - Paste your pairing phrase and set a password for this connection.

## Step 4: Set Up BTC Pay Server

1. **Access BTC Pay Server**:
   - Go back to your Voltage dashboard and click on "BTC Pay Server."
   - Click "Let's Go" and provide a name for your store.

2. **Connect with Your Node**:
   - Enter your node password to link your Lightning node with BTC Pay Server.
   - Copy the default password provided and log in to the BTC Pay Server dashboard.

3. **Account Management**:
   - Update your BTC Pay Server password for security.
   - Optionally, enable Bitcoin on-chain payments by connecting your wallet's extended public key (XPub).

## Step 5: Configure Your Payment Systems

1. **Checkout Settings**: Customize your checkout appearance via the BTC Pay Server settings.
2. **Integrate with Shopify**:
   - For integration with Shopify, refer to the [BTC Pay Server docs](https://docs.btcpayserver.org) for setup instructions.

## Step 6: Monitor Your Channels and Auto-Liquidity

1. **Check Channel Status**: 
   - Monitor the status of your channels under "Channel Analytics." Wait until your initially opened channel transitions from "pending" to "active."

2. **Enable Auto-Liquidity**: 
   - Return to your Lightning Terminal, click on "Loop," and configure it to automatically convert received Lightning funds to an on-chain wallet.

## Step 7: Expanding Your Capacity with AMBOSS

1. **Log Into AMBOSS**:
   - Go to [AMBOSS.space](https://amboss.space) and log in using your Lightning node.

2. **Set Up Notification**: 
   - Configure a notification setting to stay updated on channel offers.
   
3. **Purchase More Liquidity**:
   - Navigate to the "Magma" section to buy additional channels. Choose the size of the channel you need.

4. **Confirm Purchase**: 
   - Follow the prompts to pay for the new channel. Once paid, wait for confirmations.

## Conclusion

Congratulations! You have successfully set up a Lightning node through Voltage, connected it to BTC Pay Server, and enhanced your payment capabilities with additional liquidity. Your store is now ready to accept Lightning payments. As your business grows, monitor your channels and consider expanding your liquidity to accommodate more transactions. For ongoing support, consider joining the Voltage community.

If you have any questions or feedback, feel free to reach out. Happy building!