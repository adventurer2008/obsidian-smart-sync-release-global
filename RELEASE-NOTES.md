# Smart Sync 1.1.8

- Promote the tested Alpha.6 to the Stable channel in Hub.
- Guide signed-in accounts without a connected vault through explicit vault selection before approving another device.
- Sign-in, successful sign-in, plans, orders and payment pages inherit the plugin language without another language selector.

- Refine confirmation hints and account, plan, order and payment wording across all ten interface languages.
- Hide closed orders and empty order-status rows in My plan while preserving current plan, usage, expiry and actionable checkout/refund states. Order history remains available.

- Choose from ten interface languages, including English, Chinese, Japanese, Korean, German, French, Spanish, Portuguese and Russian. Follow Obsidian or choose a local preference, then reload the plugin.
- Use localized sign-in, plan and payment pages. Interface language does not change your account, cloud vault or billing currency.
- Pay in USD with Stripe by default; administrators can assign Dodo Payments to selected accounts or new-user scenarios. Existing orders and subscriptions keep their original provider.
- Resume an unpaid checkout instead of creating duplicates. Recover closed or initially failed Dodo orders safely, and keep uncertain payments under review.
- Verify refunds against the original payment and preserve new purchase rights when an old refund request is repeated. Correct misleading error text on refunded orders.

Synchronization, encryption, account/vault isolation and original file modification times retain their existing behavior. Replace only main.js, manifest.json and styles.css; preserve settings, secret storage, checkpoints and all vault files.
