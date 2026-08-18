# Free Custom Email Setup (contact@innocentkisoka.com)

You're using the **free version** for now. This guide focuses on the best free professional setup in 2026:

**Cloudflare Email Routing** (completely free forwarding + catch-all)

This lets you have:
- contact@innocentkisoka.com
- hello@innocentkisoka.com
- research@innocentkisoka.com
- anything@innocentkisoka.com (catch-all)

Emails forward to your existing inbox (Gmail, Proton, etc.). You can reply from the custom address using Gmail's "Send as".

---

## Step 1: Buy the Domain (innocentkisoka.com)

The domain is currently available.

**Recommended registrars (both work great with Cloudflare):**

1. **Porkbun** (often cheapest first year + excellent support)
   - Direct link: https://porkbun.com/checkout/search?query=innocentkisoka.com

2. **Cloudflare Registrar** (at-cost pricing, no markup, best for long term)
   - Go to: https://domains.cloudflare.com/
   - Search for `innocentkisoka.com`

**During purchase:**
- Enable WHOIS privacy (free on both).
- After buying, note down your domain.

---

## Step 2: Set Up Cloudflare (Free Account + DNS)

1. Go to https://dash.cloudflare.com and create a free account (or log in).

2. Click **"Add a Site"** (or "Add domain").

3. Enter `innocentkisoka.com` and click Continue.

4. Cloudflare will scan for DNS records. Click through until it gives you **two nameservers** (like `ns1.cloudflare.com` and `ns2...`).

5. **Go back to your registrar** (Porkbun or wherever you bought it) and change the nameservers to the ones Cloudflare gave you.

6. Wait 5–60 minutes for propagation (sometimes faster).

Once the domain shows as "Active" in Cloudflare, continue.

---

## Step 3: Set Up contact@innocentkisoka.com → innocentkisoka@yahoo.com

1. In your Cloudflare dashboard, select the domain **innocentkisoka.com**.

2. In the left sidebar, click **Email** → **Email Routing**.

3. If not already enabled, click **"Get Started"** and follow the prompts to enable Email Routing (Cloudflare will add the MX records automatically).

4. Click **"Create address"** (or "Manage addresses").

5. Create the exact address:
   - **Email address**: `contact`
   - **Destination email**: `innocentkisoka@yahoo.com`

   (This makes contact@innocentkisoka.com forward directly to your Yahoo inbox)

6. Click **Create**.

7. (Strongly recommended) Enable **Catch-all** so that anything@innocentkisoka.com also forwards to the same Yahoo address.

That's it. Cloudflare will now route `contact@innocentkisoka.com` (and any other addresses you create) to innocentkisoka@yahoo.com.

You should receive a test email or can send one yourself to verify.

---

## Step 4: Set Up "Send As" So You Can Reply From the Custom Address

This is important so people see `contact@innocentkisoka.com` when you reply.

### Set up "Send as" in your email client (so you can reply as contact@innocentkisoka.com)

**For Gmail (most common):**

1. Go to Gmail → Settings (gear) → **See all settings** → **Accounts and Import**

2. Under "Send mail as", click **Add another email address**

3. Fill in:
   - Name: Innocent Kisoka
   - Email: `contact@innocentkisoka.com`

4. Click Next Step → Send Verification

5. Check your Yahoo inbox (innocentkisoka@yahoo.com) for the verification code/link from Google.

6. Verify it.

After verification, you can choose `contact@innocentkisoka.com` as the "from" address when composing emails.
     - Port: 587
     - Username: your full Gmail
     - Password: App password (you may need to generate one in Google account security)

   Gmail often auto-detects Cloudflare routing for verification.

   **Option B (More reliable long-term):**
   - Once everything is set up, many people just use Gmail's "Send as" with the custom address and let Cloudflare handle it (no extra SMTP needed in many cases).

6. Click **Send Verification**. Check the inbox of `contact@innocentkisoka.com` (it will forward to your Gmail). Click the verification link.

7. After verification, go back to "Send mail as" and set `contact@innocentkisoka.com` as the **default**.

You can now send emails that appear to come from contact@innocentkisoka.com.

---

## Step 5: Update Your Portfolio & Materials

Your portfolio is already updated to use `contact@innocentkisoka.com`.

After you finish the above:

- Test by sending an email to contact@innocentkisoka.com
- Update your CV PDF (the InnocentKisokaCV.pdf file)
- Update LinkedIn, GitHub, etc.
- The contact form on your site will start delivering to the new address once DNS propagates.

---

## Quick Test

After setup, send a test email from another account to `contact@innocentkisoka.com`.

It should arrive in your main inbox within a minute or two.

---

## If You Want a Real Separate Inbox Later (Not Just Forwarding)

You can upgrade later to:
- Zoho Mail Free
- Google Workspace
- Proton Mail (paid custom domain)

But the Cloudflare routing method above is 100% free and very professional.

---

## Need Help?

Once you:
1. Buy the domain, and
2. Have Cloudflare Email Routing set up for `contact@innocentkisoka.com`

...reply here and tell me "domain is bought and routing is active", and I can:
- Double-check your portfolio code
- Help with any DNS tweaks
- Update the form action if needed
- Create additional addresses in the guide

You're all set for a clean professional email without paying monthly. Let's get the domain registered! 

Current recommended primary address: **contact@innocentkisoka.com**