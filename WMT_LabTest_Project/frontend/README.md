# Frontend - Item Manager Lab Test

## Setup
1. Open a terminal inside the frontend folder.
2. Run:
   ```bash
   npm install
   ```
3. Copy `.env.example` to `.env`
4. Start the frontend:
   ```bash
   npm run dev
   ```

## Notes
- The frontend expects the backend API at `VITE_API_URL`.
- Example:
  `VITE_API_URL=http://localhost:5000/api`

## Vercel,railway
- deploy through vercel

## If Mac Permission Denied
- 1. Make vite executable
chmod +x node_modules/.bin/vite

2. Run project
npm run dev

3. Fix all binaries
chmod -R +x node_modules/.bin

4. Clean reinstall (best fix)
rm -rf node_modules package-lock.json
npm install
npm run dev

5. Fix ownership (if used sudo before)
sudo chown -R $(whoami) .

Then reinstall:
rm -rf node_modules package-lock.json
npm install

6. Check permissions
ls -l node_modules/.bin/vite

Good output:
-rwxr-xr-x