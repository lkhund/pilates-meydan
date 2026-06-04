# Pilates Academy® Meydan — Landing Page

A single-page landing site. One file (`index.html`) holds everything — structure, styling, and the booking form.

---

## ⚡ Before it goes live — do this first

The booking form won't send anything until you connect Formspree (free):

1. Go to **formspree.io** and sign up.
2. Create a new form. It gives you an endpoint ID that looks like `xeqwabcd`.
3. Open `index.html`, find this line (around line 164 — or just search for `YOUR_FORM_ID`):

   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

4. Replace `YOUR_FORM_ID` with your real ID, then save.

Now every submission emails you. (Later you can connect Formspree → Google Sheets via Zapier.)

---

## ✏️ How to edit (in Cursor — no code knowledge needed)

1. Open this folder in Cursor: **File → Open Folder**.
2. Open `index.html`.
3. Press **Cmd/Ctrl + L** to open the AI chat.
4. Type what you want in plain English, e.g.:
   - "Change the headline to ‘Move Better, Feel Stronger’"
   - "Make the Book Now button say ‘Reserve a Spot’"
   - "Change the email to bookings@pilatesacademy.com"
   - "Swap the four classes to: Reformer, Mat, Prenatal, Private"
5. Save with **Cmd/Ctrl + S**.

### To swap in a photo
1. Drag the image file into this folder (e.g. `hero.jpg`).
2. Tell Cursor: "Use hero.jpg as the hero background image."

### To use the real logo
1. Drop your logo file in this folder (e.g. `logo.png`).
2. Tell Cursor: "Replace the crown SVG in the header and footer with logo.png."

---

## 🚀 How to deploy (Vercel — free)

### Quickest: drag & drop
1. Go to **vercel.com**, sign up (free).
2. **Add New → Project**, then use the drag-and-drop option.
3. Drag this whole folder onto it. Live in ~20 seconds at `your-project.vercel.app`.
4. To update later: drag the folder again — it redeploys.

### Smoother long-term: GitHub auto-deploy
1. Push this folder to a GitHub repo (in Cursor, press **Cmd/Ctrl + L** and ask "help me push this folder to GitHub" — it'll walk you through it).
2. On Vercel: **Add New → Project → Import** that repo.
3. From then on, every save + push auto-deploys in ~20 seconds. No re-dragging.

### Custom domain (optional)
In your Vercel project: **Settings → Domains**, add your domain (e.g. `meydan.pilatesacademy.com`). Vercel shows the DNS record to add at your registrar. SSL is automatic and free.

---

## 🎨 Brand reference (so edits stay on-brand)

**Fonts:** Cormorant Garamond (headlines), Jost (body) — loaded automatically from Google Fonts.

**Colors** (defined at the top of `index.html` under `:root`):
| Name | Hex | Use |
|------|-----|-----|
| Ink | `#2A2E33` | Main text, buttons |
| Soft | `#5C636B` | Secondary text |
| Aqua | `#7FC9C9` | Light accent |
| Aqua deep | `#3E8E8E` | Accent / hover |
| Gold | `#C9A24B` | Crown, highlights |
| Gold soft | `#D8BC7E` | Italic headline accent |
| Paper | `#FFFFFF` | Background |
| Mist | `#EEF3F3` | Section background |

To change a color everywhere, edit its value in `:root` — it updates across the whole page.

---

## 📄 Page sections (in order)
1. **Header** — logo + nav (white, sticky)
2. **Hero** — tagline + booking form
3. **Classes** — four-program grid
4. **Quote** — Joseph Pilates
5. **Visit** — Meydan CTA
6. **Footer** — links, contact, Instagram

---

*A branch of Pilates Academy® Dubai.*
