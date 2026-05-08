##  Mental Health DApp

A decentralized mental health records application built with **Next.js**, **Node.js**, **MongoDB**, and **IPFS (Pinata)**. It supports **role-based login** for Patients, Therapists, and Admins. Data is stored securely using IPFS, while access is controlled via Ethereum wallet authentication.

---

###  Features

*  **Patient**: Submit mental health records
*  **Therapist**: View records by authorized wallet address
*  **Admin**: View all records, delete them, and authorize therapists
*  Wallet-based login
*  IPFS file storage (via Pinata)
* 🢾 MongoDB for metadata storage

---

###  Tech Stack

* **Frontend**: Next.js 15, TailwindCSS
* **Backend**: Node.js (API Routes inside `pages/api`)
* **Database**: MongoDB Atlas
* **Blockchain**: Ethereum (Ethers.js)
* **Storage**: IPFS via Pinata API (JWT)

---



###  Environment Variables (`.env.local`)

```env
MONGODB_URI=mongodb+srv://<your_db_user>:<password>@<cluster-url>/<dbname>
JWT_SECRET=your_jwt_secret
PINATA_JWT=Bearer your_pinata_jwt_token
```

---

###  Setup & Development

```bash
# Install dependencies
npm install

# Run dev server
npm run dev

# Build for production
npm run build
npm start
```

---

###  Test Locally

Make sure:

* MetaMask is installed
* You’re connected to the correct network (e.g., Sepolia)
* Your wallet is added for appropriate roles (admin adds therapist)

---

###  Deployment (Vercel Recommended)

1. Go to [Vercel Dashboard](https://vercel.com)
2. Import Git repo
3. Set environment variables
4. Deploy!

If backend is separate, use [Render](https://render.com), [Railway](https://railway.app), or Heroku.

---

###  Security Notes

* Patient data is stored via IPFS; metadata stored in MongoDB
* Only authorized wallets (approved by Admin) can access sensitive therapist routes
* JWT-based secure file uploads

---
 ### No future updates
