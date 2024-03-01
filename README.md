# Next.js github page test

## 增加 next.config.js
```mjs
/** @type {import('next').NextConfig} */
const nextConfig = {
  output: "export"
};

module.exports = nextConfig
```

### 靜態檔案路徑必須為相對路徑(./image.jpg)

## github action config nextjs.yml 移除以下兩行
```
- name: Static HTML export with Next.js
  run: ${{ steps.detect-package-manager.outputs.runner }} next export
```