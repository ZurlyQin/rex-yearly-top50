# 年度高分电影 Top 50 · 2020—2025

Rex / Forward 模块，按上映年份选择 2020—2025 年，依据 TMDB 当前评分降序排列，至少 500 人评分，每年最多 50 部。默认 2025 年。

## 预览

![Rex 年度电影榜单预览](assets/yearly-top-movies-preview.jpg)

预览图中的并排卡片与标题由 Rex 首页配置；导入模块后可自行配置展示。

## 导入

在 Rex「设置 → 模块 → 通过链接添加」中输入：

```text
https://raw.githubusercontent.com/ZurlyQin/rex-yearly-top50/main/tmdb-yearly-top-movies.js
```

进入「资源库 → 年度高分电影」，展开榜单并选择上映年份。向下滚动加载，三页最多分别为 20、20 和 10 部。已安装相同 ID 模块时选择覆盖。

年份按 TMDB 主要上映年份筛选；分数随数据更新，播放资源由 Rex 资源库提供。网络请求使用 Rex 内置 TMDB 接口，无需在脚本填写密钥。

## 测试

运行 `node test-yearly-top-movies.cjs`。离线测试覆盖六个年份、评分条件、50 部上限、分页和错误处理。

This product uses the TMDB API but is not endorsed or certified by TMDB.
