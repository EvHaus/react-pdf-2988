# react-pdf-2988

This repo is to help reproduce issue: https://github.com/diegomura/react-pdf/issues/2988

Review old.pdf vs new.pdf


## Steps to reproduce

Install Bun: https://bun.sh/

- Run `bun i`
- Run `bun index.tsx`
- Open the `example.pdf` file that's generated

Note how the PDF is rendered with nice line heights.

- Run `rm -rf node_modules bun.lockb`
- Remove the `resolutions` section in `package.json`
- Run `bun i`
- Run `bun index.tsx`
- Open the `example.pdf` file that's generated

Note how the PDF is rendered with weird line heights.