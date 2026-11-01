# BD Health — demo

A static, frontend-only demo of the BD Health patient record app. Every patient, hospital and document in it is
invented; nothing is saved (a reload starts fresh). There is no server and no real data.

These files are a build output, not source. To update them, in the main app repo:

    pnpm --filter @bd/web build:demo

then replace everything here (except `.git`, `README.md` and `.gitignore`) with `apps/web/dist-demo/`, commit and push.
Vercel serves the folder as a static site: framework preset "Other", no build command, output directory `.`.
