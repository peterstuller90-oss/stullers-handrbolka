# Handrbolka Štúdio

Jednoduchá webová apka pre **Handrbolka – Lesný klub** (Trenčín). Z jedného návrhu pripraví:

- Instagram post (1080 × 1350)
- Instagram story (1080 × 1920)
- plagát A4 a A3 na tlač (PDF 300 dpi, voliteľne so spadávkou 3 mm a orezovými značkami)
- krátke intro do reelu s nadpisom a animovaným logom (MP4)

## Ako sa používa

1. Otvor apku a prihlás sa e-mailom a heslom.
2. V záložke **Obsah** napíš do poľa **Zadanie**, čo potrebuješ (napr. „Jesenná slávnosť 12. 10. o 15:00, lampióny, opekačka, príďte s rodičmi“). Apka pripraví celý návrh.
3. Ak sa ti niečo nepáči, uprav texty, pozadie, rozloženie alebo kresbičky. Tlačidlo **Nová variácia** ponúkne ďalšie rozmiestnenia.
4. **Exportovať** stiahne vybraný formát alebo všetko naraz v ZIP-e.

## Technika

- Statická stránka (GitHub Pages), bez build kroku.
- Prihlásenie, uložené návrhy a súkromný font cez Supabase (tabuľky `handrbolka_*`, prístup len pre povolené e-maily cez RLS).
- Písmo Goldplay Alt je platené, preto **nie je v tomto repozitári**. Apka ho po prihlásení načíta zo Supabase.
- Automatický návrh zo zadania používa Supabase Edge Function `handrbolka-brief`. Kým nie je nasadená, apka pripraví jednoduchší návrh priamo v prehliadači.
