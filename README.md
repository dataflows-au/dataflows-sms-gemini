<img src="assets/icon.png" alt="DataFlows SMS" width="96">

# DataFlows SMS for Gemini CLI

Send, schedule and track business SMS from your DataFlows account by asking Gemini in plain language. The extension connects Gemini CLI to the DataFlows SMS MCP server and adds guidance so Gemini confirms every send, previews cost and compliance warnings before contact group campaigns, and reports delivery and replies clearly.

## What you need

* A [DataFlows](https://dataflows.com.au) account with SMS credits
* A sender ID or number on your account
* [Gemini CLI](https://geminicli.com)

## Install

```bash
gemini extensions install https://github.com/dataflows-au/dataflows-sms-gemini
```

Then start Gemini CLI and sign in to DataFlows:

```
/mcp auth dataflows-sms
```

Your browser opens the DataFlows sign-in page. Sign in with your DataFlows login and select **Allow Access**.

Using Antigravity CLI? Install the extension with Gemini CLI as above, then run `agy plugin import gemini` to bring it across.

## Use it

Ask Gemini things like:

* "What's my DataFlows SMS balance and which sender IDs can I use?"
* "Send 'Your order is ready for pickup' to 0412 345 678 from DataFlows."
* "Preview a message to my Demo customers group saying 'We're closed on Monday for the public holiday', then send it once I confirm."
* "Schedule 'Reminder: your appointment is tomorrow at 10am' to 0412 345 678 for 9am tomorrow."
* "Did my messages today get delivered, and did anyone reply?"

Gemini asks you to confirm before any message is sent. The same sender ID registration, opt-out and blocklist rules as the DataFlows dashboard apply.

## What's included

* **MCP server**: `https://sms.dataflows.com.au/mcp/gemini`, with tools to check your balance and senders, preview, send and schedule messages, and read delivery status, replies, campaign results and usage.
* **GEMINI.md**: the confirm and preview workflow for sending and scheduling, and how to report on delivery, replies, campaigns and usage.

## Data

The extension itself stores nothing and runs no code. Everything goes through the DataFlows SMS MCP server at `sms.dataflows.com.au`, which acts only on the DataFlows account you sign in with, and only when you ask. It sends the phone numbers, message text, sender and send time you give it to DataFlows, and returns your balance, senders, contact group names and sizes, and the status and replies of messages sent through this connection. Messages are delivered by DataFlows' carrier partners. See the [DataFlows Privacy Policy](https://dataflows.com.au/privacy-policy), section "AI Assistant Connections".

## Support

Email [support@dataflows.com.au](mailto:support@dataflows.com.au).

## License

MIT License. See [LICENSE](LICENSE).
