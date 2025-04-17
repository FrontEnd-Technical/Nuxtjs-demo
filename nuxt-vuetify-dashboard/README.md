# Tạo Project
## Khởi tạo project nuxt

```bash
npm create nuxt <project-name>
```

## Tích hợp tailwind

```bash
# Install Tailwind CSS
npm install tailwindcss @tailwindcss/vite

# Create an ./assets/css/main.css file and add an @import that imports Tailwind CSS
[main.css] @import "tailwindcss";

#Configure [nuxt.config.ts] file

    import tailwindcss from "@tailwindcss/vite";
    export default defineNuxtConfig({
    compatibilityDate: "2024-11-01",
    devtools: { enabled: true },
    css: ['~/assets/css/main.css'],
    vite: {
        plugins: [
        tailwindcss(),
        ],
    },
    });

```