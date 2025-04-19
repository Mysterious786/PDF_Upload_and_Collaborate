# 📚 PDF Upload and Collaborate

A full-featured web application for uploading, viewing, and collaborating on PDF files. Built using **Next.js**, **TypeScript**, **Tailwind CSS**, and modern development practices. Users can securely log in, upload PDFs, and share them with others for real-time collaboration.  
🔗 **Live Demo**: [pdf-upload-and-collaborate.vercel.app](https://pdf-upload-and-collaborate.vercel.app)

## Features

- 🔐 User Authentication – Secure login and registration  
- 📤 Upload PDFs – Upload and manage PDF files  
- 👥 Real-Time Collaboration – Collaborate on documents (coming soon)  
- 🌐 Public & Private Sharing – Control access to your uploads  
- 🧠 Context API – Manage global state like authentication and uploads  
- 📱 Fully Responsive – Works great on mobile, tablet, and desktop  

## Tech Stack

**Frontend:** Next.js, TypeScript, Tailwind CSS  
**Backend:** Next.js API Routes (Serverless)  
**State Management:** React Context API  
**Cloud Storage:** Cloudinary  
**Deployment:** Vercel  

## Folder Structure

```
PDF_Upload_and_Collaborate/
├── app/                 # App routes and pages (Next.js 13+)
├── components/          # Reusable UI components
├── context/             # Auth and global context providers
├── hooks/               # Custom React hooks
├── lib/                 # Utility functions (e.g., Cloudinary logic)
├── models/              # Type definitions and models
├── public/              # Static assets
├── styles/              # Global and custom styles
├── .env.local           # Environment variables (not committed)
├── next.config.mjs      # Next.js configuration
├── tailwind.config.ts   # Tailwind CSS configuration
├── tsconfig.json        # TypeScript configuration
└── README.md            # This file!
```

## Getting Started

Clone the repository:  
```bash
git clone https://github.com/Mysterious786/PDF_Upload_and_Collaborate.git
cd PDF_Upload_and_Collaborate
```

Install dependencies:  
```bash
# using pnpm
pnpm install
# or using yarn
yarn install
```

Add environment variables in `.env.local`:
```env
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_UPLOAD_PRESET=your_upload_preset
```

Run the development server:  
```bash
pnpm dev
# or
yarn dev
```

Visit `http://localhost:3000` to view the app.

## Cloudinary Integration

PDFs are uploaded from the frontend directly to Cloudinary using a secure unsigned preset. Once uploaded, the file URL is stored and displayed using a PDF preview component.

## Deployment

Deployed using **Vercel**. To deploy your own version:

1. Push the repo to GitHub  
2. Connect it with Vercel  
3. Add your environment variables  
4. Deploy with one click  

## Future Improvements

- 🔁 Real-time document collaboration (Socket.IO or Pusher)  
- 🗃️ Folder-based file organization  
- 🔍 PDF content search  
- 📨 Invite users via email  
- 🔐 OAuth login (Google, GitHub)  
- 📝 Inline commenting and annotations  

## Contributing

Contributions are welcome!  
1. Fork the project  
2. Create a new branch: `git checkout -b feature/my-feature`  
3. Make your changes  
4. Commit: `git commit -m 'Add my feature'`  
5. Push: `git push origin feature/my-feature`  
6. Open a pull request  

## License

This project is licensed under the **MIT License**. See `LICENSE` file for details.

## Author

Made with ❤️ by **Mysterious786**  
GitHub: [github.com/Mysterious786](https://github.com/Mysterious786)
