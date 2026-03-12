# Frontend linting setup

1) Что добавить
- `package.json` — скрипты `lint`, `format`, `prepare`.
- `.eslintrc.json`, `.prettierrc` — базовые конфиги.
- `husky` + `lint-staged` — локальные pre-commit хуки.

2) Быстрая установка

```bash
cd frontend
npm install --save-dev eslint prettier husky lint-staged @typescript-eslint/parser @typescript-eslint/eslint-plugin
npm run prepare
npx husky add .husky/pre-commit "npx lint-staged"
```

3) Проверка

```bash
npm run lint
npm run format
npx lint-staged --verbose
```
