# kaimengzhifang-assets

开蒙纸坊（https://ohmynotes.com）用到的大体积静态资源，单独放在这个公开仓库里，由 jsDelivr 当 CDN 分发：

```
https://cdn.jsdelivr.net/gh/iForcecome/kaimengzhifang-assets@<提交号>/bg/qianli.jpg
```

- `bg/`：四幅公有领域名画扫描（千里江山图、富春山居图、溪山行旅图、早春图），来源与许可见 `bg/README.md`；已缩到 1200 到 1400 像素宽、质量 70，做纸张淡底用。
- `fonts/`：PDF 导出时嵌入的霞鹜文楷子集（OFL 许可，见 `fonts/LXGW-WenKai-OFL.txt`）。

主仓库的 `deploy/deploy.sh` 构建前会取这个仓库 `main` 的最新提交号，把前端里的资源基址指到它；换图只要往这里推，再发一次版即可。
