# 🛡 Security & Privacy

## Secrets
- `GEMINI_API_KEY` is stored in environment variables (`.env.local` locally, Vercel settings in production).
- Keys are used only on the server and never sent to the browser.
- `.env*` files are listed in `.gitignore`. **Never commit them.**

## Uploads
- Allowed types: PDF, DOC, DOCX, PPT, PPTX, TXT, CSV, XLS, XLSX, JPG, PNG.
- Maximum size: 50 MB.
- Uploaded material is used only to generate the student's own study content.

## Responsible AI
- Content is grounded in the student's document.
- No invented progress statistics.
- Students should cross-check important facts.

## Reporting a vulnerability
Please open a private report via the repository's **Security** tab, or contact the maintainer on GitHub: [@amrut4469-blip](https://github.com/amrut4469-blip).
