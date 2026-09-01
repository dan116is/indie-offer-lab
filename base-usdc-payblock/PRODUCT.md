# Base USDC Pay Block (copy-paste for indie landings)

**SKU:** `base-usdc-payblock`  
**Price:** $5 USD, paid in USDC on Base  
**Format:** Original landing copy + HTML snippet + operator checklist

This is original instructional copy for **receiving USDC on Base**. It is not a wallet, not a payment processor, not a smart-contract product, and not Coinbase’s docs. It does not move funds for you.

**Not financial, tax, or legal advice.**

## Facts you must not blur

| Fact | Value |
|---|---|
| Network | Base |
| Chain id | 8453 |
| Asset | USDC (Circle-issued on Base) |
| Canonical USDC contract on Base | `0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913` |
| Receiving address (this lab) | `0xeC128EDD43DF3DC8a87d6A53C7506A3D6037B9c4` |
| Memo | **Not on-chain.** Put `memo=[slug]` in the email. |
| Orders inbox | `agent-0af2826d2bd111cc@agentmail.to` |
| Explorer | https://basescan.org |

When you reuse this HTML on *your* site, substitute *your* address in the hero, terms, and email.

## Buyer-facing copy

```
Pay with USDC on Base

1. Open a wallet that supports Base (chain id 8453).
2. Send exactly [PRICE] USDC. Token contract:
   0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913
3. To:
   0xeC128EDD43DF3DC8a87d6A53C7506A3D6037B9c4
4. There is no on-chain memo. Do not look for a memo field.
5. Email the transaction hash to
   agent-0af2826d2bd111cc@agentmail.to
   Subject: ORDER [slug]
   Body: hash, BaseScan link, the address you sent from, slug=[slug]

Wrong network or wrong token is not a completed order. Recovery is not promised.
If you need a test, send nothing — email a question first.
```

Button label (not a fake card charge):

```
Pay [PRICE] USDC on Base — then email the hash
```

## HTML snippet (no third-party script)

```html
<section id="pay" style="border:1px solid #0f766e;border-radius:12px;padding:1rem 1.1rem;max-width:36rem;font-family:system-ui,sans-serif">
  <h2 style="margin-top:0">Pay — USDC on Base</h2>
  <p>Amount: <strong>[PRICE] USDC</strong> · Network: <strong>Base</strong> · Chain id <code>8453</code></p>
  <p>Send to:</p>
  <p><code>0xeC128EDD43DF3DC8a87d6A53C7506A3D6037B9c4</code></p>
  <p>USDC token (Base):<br/>
  <code>0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913</code></p>
  <p>Memo: email only. Use slug <code>[slug]</code>.</p>
  <p>After send, email hash to
    <a href="mailto:agent-0af2826d2bd111cc@agentmail.to?subject=ORDER%20[slug]">agent-0af2826d2bd111cc@agentmail.to</a>
  </p>
  <p style="font-size:.9rem;color:#57534e">Do not send ETH-mainnet USDC, USDT, or Base ETH as the product price.</p>
</section>
```

## Wallet UI coaching

1. Network dropdown says **Base**, not Ethereum, not Base Sepolia.
2. Token picker says **USDC**, not USDbC, not USDT, not ETH.
3. Amount equals the listing. Gas is separate (ETH on Base).
4. Paste the address; confirm first 6 and last 4 characters.
5. After send, paste hash into BaseScan. Confirm token, amount, and `to` before you email.

Sepolia / testnet USDC is not payment.

## Operator checklist (after email arrives)

- [ ] Hash resolves on **basescan.org**, not etherscan.io
- [ ] Token is `0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913`
- [ ] `to` is your receiving address
- [ ] Amount ≥ listed price
- [ ] Explorer shows success — do not fulfill on a mempool screenshot
- [ ] Slug in subject matches a real SKU
- [ ] Reply with the files; keep the hash in your records

Underpay: email the shortfall. Do not ship a pro-rated file unless you said you would.

## FAQ under the pay block

**Can I add a memo in MetaMask?** Not for ERC-20 USDC. Use the order email.

**Can I pay with ETH and you’ll convert?** No. The listing is USDC.

**Coinbase centralized send?** Only if the withdrawal network is Base and the asset is USDC to the exact address. If Coinbase asks for a memo/tag, stop and re-read.

**Do you watch the chain automatically?** This pack assumes a human reads the orders inbox. Do not pretend a watcher exists.

## What this pack is not

Not escrow, not KYC, not “onchain commerce infrastructure,” not permission to spam wallets, not a reason to invent volume numbers.

## Pay this pack

Send **$5 USDC on Base** to `0xeC128EDD43DF3DC8a87d6A53C7506A3D6037B9c4`.  
Email `ORDER base-usdc-payblock` + tx hash to `agent-0af2826d2bd111cc@agentmail.to`.
