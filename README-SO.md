# Maqaayad App — Android, iPhone iyo Computer

## Waxa ku jira
- `server.js`: server-ka iyo app-ka.
- `package.json`: dependencies iyo amarka bilowga.
- PWA manifest iyo service worker oo ku jira server-ka.

## Ku tijaabi computer
1. Ku rakib Node.js 18 ama ka cusub.
2. Fur terminal gudaha galkaan.
3. Ku rakib dependencies: `npm install`.
4. Nuqul ka samee `.env.example` oo u bixi `.env`.
5. Beddel `ADMIN_PASSWORD` una samee password adag.
6. Orod: `npm start`.
7. Fur `http://localhost:3000`.

## Ku rakib qalabka kale
App-ka waa in marka hore lagu daabacaa hosting leh HTTPS. Kadib:
- Android: Chrome ku fur link-ga, dooro Install app ama Add to Home screen.
- iPhone: Safari ku fur link-ga, taabo Share, kadib Add to Home Screen.
- Windows/macOS/Linux: Chrome ama Edge ku fur, dooro Install app (haddii browser-ku muujiyo).

## Muhiim
- PWA-gu wuxuu ka shaqayn karaa Android, iPhone iyo computer hal codebase. Ma aha APK ama App Store app native ah.
- Xogta dalabyada, menu-ga iyo maamulka waxay u baahan yihiin internet iyo server shaqaynaya. Service worker-ku wuxuu kaydiyaa app shell-ka si boggu u furmi karo offline, balse ma kaydiyo ama ma sync-gareeyo API data offline.
- Hosting-ka waa inuu leeyahay HTTPS iyo persistent disk (`DATA_DIR`) ama Supabase. Haddii hosting-ku tirtirayo filesystem-ka marka restart dhaco, xogta local way lumi kartaa.
- `ORDERS_PASSWORD` haddii aan la dejin, dalabyada cusub waa public sida uu code-ka asalka ahi u qorsheeyay. Haddii aad rabto in akhrinta liiska dalabyada la ilaaliyo, dejiso password-kan.
- `SUPABASE_KEY` waxaa isticmaala server-ka oo keliya; ha gelin browser-ka.
