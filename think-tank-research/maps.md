# 地图思路

## 三种形式

1. **着色地图（choropleth）**：按国家上色。例：各国通胀率、贸易依存度、KOF 指数。可以加年份滑块看变化。
2. **流向地图（flow map）**：国家之间画弧线，粗细 = 贸易额。例：原油主要出口国 → 进口国。最能体现"全球化"。
3. **气泡地图**：在国家中心画圆，大小 = 数值。例：石油产量。

## 底图资源

- world-atlas（TopoJSON，D3 官方维护）：https://github.com/topojson/world-atlas
  - 110m 精度：`https://cdn.jsdelivr.net/npm/world-atlas@2/countries-110m.json`
- Natural Earth（原始矢量数据）：https://www.naturalearthdata.com/

## 技术（对应 my-vis-5609 的 Svelte + D3）

- `d3-geo`：投影（`geoNaturalEarth1` / `geoEqualEarth`）和 `geoPath`
- `topojson-client`：把 TopoJSON 转成 GeoJSON
- 注意：world-atlas 的国家 id 是 ISO 数字代码（如 `840` = 美国），和 World Bank 的 ISO3 字母代码需要一张对照表。
