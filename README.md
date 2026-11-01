# KHAAN'S DIGITS

The website for KHAAN'S DIGITS: personalised digital cards for special occasions, with a three-step order wizard that sends each order to WhatsApp.

Built with Next.js 16 (App Router), React 19, TypeScript, Tailwind CSS 4 and shadcn/ui.

## Requirements

- [Node.js](https://nodejs.org) 20.9 or newer
- [pnpm](https://pnpm.io/installation) (recommended). npm also works.

## Install and run

1. Extract the ZIP and open the folder in VS Code (**File > Open Folder…**).
2. Open the terminal (**Terminal > New Terminal**) and install the dependencies:

   ```bash
   pnpm install
   ```

   With npm, use `npm install` instead.

3. Start the development server:

   ```bash
   pnpm dev
   ```

4. Open http://localhost:3000 in your browser.

## Production build

```bash
pnpm build
pnpm start
```

## Where to edit business details

| What | File |
| --- | --- |
| Package prices, delivery fees, payment accounts, WhatsApp number, business email | `lib/catalog.ts` |
| WhatsApp order message | `lib/order.ts` |
| Photo and video upload limits | `lib/order-media.ts` |
| FAQs, reviews and services text | `lib/site-content.ts` |
| Order wizard screens | `components/studio/order/` |
| Header and footer | `components/studio/site-shell.tsx` |

## Payment details

- **Easypaisa (Pakistan):** Nosheen Zaman, 03170507839
- **SadaPay (international):** 03449531512
- **WhatsApp:** 0344 9531512
- **Email:** ibraheemimran938@gmail.com

## How orders work

The site doesn't take payments, and it doesn't save orders or files. Photos, videos and payment receipts are previewed only in the customer's browser. When the order is finished, the site opens WhatsApp with the full order summary filled in, and the customer attaches their files in that chat.

## Deploy

Push the project to GitHub and import it on [Vercel](https://vercel.com/new). No environment variables are needed.
