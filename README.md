# Vue 3 + TypeScript + Vite v3.0.0-alpha-6

https://github.com/vitejs/vite/pull/8358

**Vue3: npm create vite vite-3-alpha-6-test -- --template vue-ts**

Using `pnpm 7.1.6` with `corepack`, versions tested:
- Vite ^2.9.9, Vue ^3.2.36 and @vitejs/plugin-vue ^2.3.3
- Vite 3.0.0-alpha.6, Vue ^3.2.36 and @vitejs/plugin-vue ^2.3.3 (exact version for Vite)
- Vite 3.0.0-alpha.6, Vue ^3.2.36 and @vitejs/plugin-vue 3.0.0-alpha.1 (exact version for Vite and @vitejs/plugin-vue)

The results can be found comparing `dist-vite-**/assets/index.XXXX.js`, not minified:
- folder dist-vite-2.9.9
- folder dist-vite-3.a.6
- folder dist-vite-3.a.6-p-3.a.1

<details>
<summary><strong>VUE 3.2.36/VITE 2.9.9/VUE PLUGIN 2.3.3</strong></summary>

```shell
F:\work\projects\quini\GitHub\vite-3-alpha-6-tests\vite-3-alpha-6-test>pnpm run build

> vite-3-alpha-6-test@0.0.0 build F:\work\projects\quini\GitHub\vite-3-alpha-6-tests\vite-3-alpha-6-test
> vue-tsc --noEmit && vite build

vite v2.9.9 building for production...
✓ 14 modules transformed.
dist/assets/logo.03d6d6da.png    6.69 KiB
dist/index.html                  0.42 KiB
dist/assets/index.89b33d7f.css   0.41 KiB / gzip: 0.27 KiB
dist/assets/index.878eb311.js    143.96 KiB / gzip: 32.35 KiB
```
</details>

<details>
<summary><strong>VUE 3.2.36/VITE 3.0.0-alpha.6/VUE PLUGIN 2.3.3</strong></summary>

```shell
F:\work\projects\quini\GitHub\vite-3-alpha-6-tests\vite-3-alpha-6-test>pnpm run build

> vite-3-alpha-6-test@0.0.0 build F:\work\projects\quini\GitHub\vite-3-alpha-6-tests\vite-3-alpha-6-test
> vue-tsc --noEmit && vite build

vite v3.0.0-alpha.6 building for production...
✓ 10 modules transformed.
dist/assets/logo.03d6d6da.png    6.69 KiB
dist/index.html                  0.42 KiB
dist/assets/index.89b33d7f.css   0.41 KiB / gzip: 0.27 KiB
dist/assets/index.a236cc27.js    160.73 KiB / gzip: 38.03 KiB
```
</details>

<details>
<summary><strong>VUE 3.2.36/VITE 3.0.0-alpha.6/VUE PLUGIN 3.0.0-alpha.1</strong></summary>

```shell
F:\work\projects\quini\GitHub\vite-3-alpha-6-tests\vite-3-alpha-6-test>pnpm run build

> vite-3-alpha-6-test@0.0.0 build F:\work\projects\quini\GitHub\vite-3-alpha-6-tests\vite-3-alpha-6-test
> vue-tsc --noEmit && vite build

vite v3.0.0-alpha.6 building for production...
✓ 12 modules transformed.
dist/assets/logo.03d6d6da.png    6.69 KiB
dist/index.html                  0.42 KiB
dist/assets/index.06df8542.css   0.41 KiB / gzip: 0.27 KiB
dist/assets/index.efb834ec.js    160.73 KiB / gzip: 38.02 KiB
```
</details>



