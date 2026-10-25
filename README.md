# Customer Angular (Firstproject)

Angular 15 learning project that demonstrates core Angular features: routing with a 404 page, data binding, template-driven forms, a customer details view, a product list loaded from the public [Fake Store API](https://fakestoreapi.com/products) with Angular Material dialogs, and client-side pagination with `ngx-pagination`.

## Tech stack

- Angular 15 (Angular CLI 15.0), TypeScript
- Angular Material 15, Bootstrap 5
- ngx-pagination

## Folder structure

```text
Customer-Angular/
├── .vscode/
├── src/
│   ├── app/
│   │   ├── about/
│   │   ├── customer-details/
│   │   ├── data-binding/
│   │   ├── delete-dialog/
│   │   ├── home/
│   │   ├── my-form/
│   │   ├── name-editer/
│   │   ├── pagenotfound-component/
│   │   ├── pagination/
│   │   └── product/
│   ├── assets/
│   ├── index.html
│   └── main.ts
├── .editorconfig
├── .gitignore
├── angular.json
├── package-lock.json
├── package.json
├── README.md
├── tsconfig.app.json
├── tsconfig.json
└── tsconfig.spec.json
```

| Path | Purpose |
| --- | --- |
| `src/app/home`, `about` | Simple pages |
| `src/app/product` | Product list (Fake Store API) and `ProductService` |
| `src/app/pagination` | Paginated product table loaded from the Fake Store API (`/fakeapi` route); `db.json` holds sample data that the code does not currently use |
| `src/app/customer-details` | Customer model, sample data and details component |
| `src/app/data-binding`, `my-form`, `name-editer` | Data-binding and forms examples |
| `src/app/delete-dialog` | Material confirmation dialog |
| `src/app/pagenotfound-component` | Wildcard (404) route |

Routes: `/` and `/home`, `/products`, `/about`, `/fakeapi`, and `**` (not found).

## Prerequisites

- Node.js 14.20+, 16.13+ or 18.10+ (supported by Angular 15) and npm
- Internet access for the product page (Fake Store API)

## Running locally

```bash
npm install
npm start          # ng serve → http://localhost:4200
```

## Build and test

```bash
npm run build      # output in dist/
npm test           # Karma + Jasmine
```
