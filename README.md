━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  🍽  THE SAFFRON TABLE — DIGITAL MENU + QR SYSTEM
        Demo by VisualMind AI | Zero Cost Setup
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

WHAT'S IN THIS FOLDER
──────────────────────
  index.html   → The restaurant menu (show this to guests via QR)
  admin.html   → Admin panel for restaurant owner (manage menu, generate QR codes)
  README.txt   → This file

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  STEP 1 — CUSTOMISE THE MENU (index.html)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Open index.html in any text editor (Notepad, VS Code etc.)

CHANGE RESTAURANT NAME:
  Search: "The Saffron Table"
  Replace with your restaurant name

CHANGE MENU ITEMS:
  Find the MENU = { ... } section in the <script>
  Each item looks like this:
    { id: 'unique-id', name: 'Dish Name', emoji: '🍛', veg: true,
      desc: 'Description of the dish',
      price: 280, originalPrice: null,  ← null = no strikethrough
      ingredients: ['Item1','Item2','Item3'],
      allergens: ['Dairy','Nuts'],  ← or [] if none
      spice: '🌶 Medium',  ← 🌶 Mild / 🌶 Medium / 🌶🌶 Spicy / —
      tags: ['bestseller'],  ← bestseller / new / special (or [])
      customise: []  ← options like [{label:'Extra Spicy',extra:0}]
    }

CHANGE WHATSAPP NUMBER (for order notifications):
  Search: const waNumber = '919876543210'
  Replace with your number (91 + 10 digit mobile, no spaces)

CHANGE TABLE NUMBER:
  Search: "Table 7" (appears in hero and cart)
  Each table gets its own QR with ?table=1, ?table=2 etc (admin generates these)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  STEP 2 — HOST IT FREE ONLINE (Required for QR to work)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

The menu needs to be online so guests can open it via QR.

EASIEST METHOD — Netlify Drop (30 seconds):
  1. Go to: https://app.netlify.com/drop
  2. Drag your entire folder onto the page
  3. You get a free URL like: https://charming-dish-123.netlify.app
  4. Done! Share this URL to generate QR codes.

OTHER FREE OPTIONS:
  • Tiiny.host → upload the ZIP, get instant link (no account needed)
  • GitHub Pages → free, permanent, professional

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  STEP 3 — GENERATE QR CODES (admin.html)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  1. Open admin.html in your browser
  2. Click "QR Code Setup" in the left menu
  3. Paste your live menu URL
  4. Click "Generate QR"
  5. QR codes for Tables 1–8 appear automatically
  6. Click "Print All QR Codes"
  7. Cut out each QR, laminate it, place on tables

Or use QR Code Monkey app on iPhone:
  1. Open app → Enter your URL
  2. Set colour to match your restaurant
  3. Download + print

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  HOW ORDERS WORK
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  Guest scans QR → Menu opens on phone
  Guest taps items → Adds to cart → Places order
  Order summary opens WhatsApp → Sent to restaurant number
  Kitchen gets the WhatsApp message

  The order message format:
  ──────────────────────────────
  🛎 New Order — Table 7
  🍛 Dal Makhani ×2 (Extra Butter) — ₹680
  🫓 Butter Naan ×3 — ₹180
  💰 Total: ₹860
  📝 Instructions: Less spicy please
  ──────────────────────────────

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  FEATURES IN THIS DEMO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✓ Works on iOS and Android (any browser)
  ✓ No app install needed — opens in browser
  ✓ Rotating promo banner (auto-slides)
  ✓ Chef's Specials horizontal scroll section
  ✓ 3 offer banners (customisable)
  ✓ Complimentary items section
  ✓ 5 menu categories (27 items total)
  ✓ Veg / Non-veg indicators (FSSAI compliant)
  ✓ Spice level tags
  ✓ Bestseller / New / Chef's Pick badges
  ✓ Item detail modal with full ingredients
  ✓ Allergen warnings
  ✓ Customisation options per item (size, spice etc)
  ✓ Add-to-cart with quantity control
  ✓ Special note per item
  ✓ Cart with subtotal, GST, service charge
  ✓ Kitchen instructions note field
  ✓ WhatsApp order delivery
  ✓ Dark luxury aesthetic — works beautifully at night

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  WHAT TO CHARGE YOUR CLIENTS (YOUR BUSINESS)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  Basic Package   → ₹2,500 setup + ₹399/month
  Standard        → ₹4,000 setup + ₹599/month
  Premium         → ₹6,500 setup + ₹999/month

  This demo file = your portfolio piece. Show it to every
  restaurant owner on your iPhone. Say: "Your menu will
  look exactly like this."

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  BUILT BY: VisualMind AI | POWERED BY: Claude (Anthropic)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
