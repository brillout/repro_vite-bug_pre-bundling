Generated with [vike.dev/new](https://vike.dev/new) ([version 493](https://www.npmjs.com/package/create-vike/v/0.0.493)) using this command:

```sh
pnpm create vike@latest --react --compiled-css --mantine --telefunc --hono --prisma --cloudflare --eslint --prettier
```

## Contents

* [*Prisma*](#prisma)

  * [Setup](#setup)

* [Photon](#photon)

  * [Plus files](#plus-files)
  * [Routing](#routing)
  * [SSR](#ssr)
  * [HTML Streaming](#html-streaming)

* [Mantine](#mantine)

## *Prisma*

### Setup

Run the following command once:

```sh
pnpx prisma init
```

then follow instructions at <https://www.prisma.io/docs/getting-started/quickstart#2-model-your-data-in-the-prisma-schema>

## Photon

[Photon](https://photonjs.dev) is a next-generation server and deployment toolkit.
It supports popular deployments ([self-hosted](https://photonjs.dev/self-hosted), [Cloudflare](https://photonjs.dev/cloudflare), [Vercel](https://photonjs.dev/vercel), and [more](https://photonjs.dev/deploy))
and popular servers ([Hono](https://photonjs.dev/hono), [Express](https://photonjs.dev/express), [Fastify](https://photonjs.dev/fastify), and [more](https://photonjs.dev/server)).

This app is ready to start. It's powered by [Vike](https://vike.dev) and [React](https://react.dev/learn).

### Plus files

[The + files are the interface](https://vike.dev/config) between Vike and your code.

* [`+config.ts`](https://vike.dev/settings) — Settings (e.g. global default `<title>`)
* [`+Page.tsx`](https://vike.dev/Page) — The `<Page>` component
* [`+data.ts`](https://vike.dev/data) — Fetching data (for your `<Page>` component)
* [`+Layout.tsx`](https://vike.dev/Layout) — The `<Layout>` component (wraps your `<Page>` components)
* [`/pages/_error/+Page.tsx`](https://vike.dev/error-page) — The error page (rendered when an error occurs)
* [`+onPageTransitionStart.ts`](https://vike.dev/onPageTransitionStart) and `+onPageTransitionEnd.ts` — For page transition animations
* [`+Head.tsx`](https://vike.dev/Head) - Sets `<head>` tags

### Routing

[Vike's built-in router](https://vike.dev/routing) lets you choose between:

* [Filesystem Routing](https://vike.dev/filesystem-routing) (the URL of a page is determined based on where its `+Page.jsx` file is located on the filesystem)
* [Route Strings](https://vike.dev/route-string)
* [Route Functions](https://vike.dev/route-function)

### SSR

SSR is enabled by default. You can [disable it](https://vike.dev/ssr) for all or specific pages.

### HTML Streaming

You can [enable/disable HTML streaming](https://vike.dev/stream) for all or specific pages.

## Mantine

This is a boilerplate for Mantine based on the [Getting Started](https://mantine.dev/docs/getting-started/) guide.

The following Packages are installed:

* `@mantine/hooks` Hooks for state and UI management
* `@mantine/core` Core components library: inputs, buttons, overlays, etc.

If you add more packages, make sure to update the `layouts/LayoutDefault.tsx` file to include the required CSSs.

The theme is defined in `layouts/theme.ts`.

