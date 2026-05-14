# 개인 홈페이지

Astro 기반 개인 홈페이지 프로젝트입니다.

최종 배포 목표는 GitHub Pages의 `github.io` 주소입니다.

## 프로젝트 구조

현재 첫 버전은 Home 페이지만 포함합니다. 이후 About, Projects, Posts 페이지로 확장할 수 있습니다.

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro는 `src/pages/` 폴더의 `.astro` 또는 `.md` 파일을 페이지로 인식합니다.

예상 확장 구조:

```text
src/
├── pages/
│   ├── index.astro
│   ├── about.astro
│   ├── projects.astro
│   └── posts/
│       └── index.astro
├── components/
└── layouts/
```

정적 파일은 `public/` 폴더에 둘 수 있습니다.

## 명령어

모든 명령은 프로젝트 루트에서 실행합니다.

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
