# pr-flow-story

סקיל לסוכני קוד (Claude Code, Cursor, Codex, Copilot ודומים) שממפה PR גדול — במיוחד כזה שנכתב עם AI — ל־**סיפור**, **דיאגרמת זרימה מלמעלה למטה (לפני/אחרי)**, ו־**מדריך במה להתמקד**.

מבוסס על חלק 3 בסדרה של TomerCode על קוד־ריוויו בעידן ה־AI: קודם מבינים את התמונה, מתמקדים בדיזיין ובהפרדת תלויות, ורק אחר כך צוללים לשורות. פונקציות עלים קל יותר לתקן אחר כך; טעויות ארכיטקטורה עולות ביוקר.

## מה יוצא בפועל

1. סיפור ה־PR — למה, מי מפעיל, happy path, סיכונים  
2. Mermaid — flow לפני ואחרי, מלמעלה למטה  
3. Focus — מה לקרוא שורה־שורה ומה לדפדף  
4. בדיקת פיצול — מתי לבקש סטאק של PRים קטנים ([stacked-pr-split](https://github.com/TomerCohen95/stacked-pr-split))

## התקנה

להעתיק את התיקייה לתיקיית הסקילים של הסוכן (למשל `~/.claude/skills/pr-flow-story/` או `.agents/skills/pr-flow-story/`). הקובץ המרכזי הוא [`SKILL.md`](./SKILL.md).

## סקילים קשורים

- [stacked-pr-split](https://github.com/TomerCohen95/stacked-pr-split) — פיצול ל־PRים מוערמים כשהסיפור לא נכנס לריוויו אחד.
- [visual-explainer](https://github.com/nicobailon/visual-explainer) — HTML / שקפים / `/diff-review` להסבר ויזואלי עשיר של אותו שינוי. התקנה: `npx skills add nicobailon/visual-explainer`.
- אופציונלי: [PR Lens](https://github.com/coldteadotai/pr-lens) — ווקהטרו של ארכיטקטורה בתוך ה־PR.

## רישיון

MIT.
