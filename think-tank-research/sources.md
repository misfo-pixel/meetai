# 数据来源清单

## 经济 / 能源（已在用的类型）

| 指标 | 来源 | 链接 |
|------|------|------|
| WTI 原油价格（日） | FRED `DCOILWTICO` | https://fred.stlouisfed.org/series/DCOILWTICO |
| Brent 原油价格（日） | FRED `DCOILBRENTEU` | https://fred.stlouisfed.org/series/DCOILBRENTEU |
| 美国 CPI | FRED `CPIAUCSL` | https://fred.stlouisfed.org/series/CPIAUCSL |
| 各国通胀率 | World Bank `FP.CPI.TOTL.ZG` | https://data.worldbank.org/indicator/FP.CPI.TOTL.ZG |
| 能源生产/消费/贸易 | 美国 EIA | https://www.eia.gov/opendata/ |
| 全球能源统计 | Energy Institute Statistical Review（原 BP 年鉴） | https://www.energyinst.org/statistical-review |

## 全球化 / 贸易

| 指标 | 来源 | 链接 |
|------|------|------|
| 贸易占 GDP 比重 | World Bank `NE.TRD.GNFS.ZS` | https://data.worldbank.org/indicator/NE.TRD.GNFS.ZS |
| FDI 净流入占 GDP | World Bank `BX.KLT.DINV.WD.GD.ZS` | https://data.worldbank.org/indicator/BX.KLT.DINV.WD.GD.ZS |
| 双边贸易流（国家×国家×商品） | UN Comtrade | https://comtradeplus.un.org/ |
| 关税、贸易统计 | WTO Stats | https://stats.wto.org/ |
| KOF 全球化指数（经济/社会/政治） | ETH Zürich KOF | https://kof.ethz.ch/en/forecasts-and-indicators/indicators/kof-globalisation-index.html |
| 增加值贸易 / 供应链 | OECD TiVA | https://www.oecd.org/en/topics/sub-issues/trade-in-value-added.html |
| 整理好的图表和数据 | Our World in Data | https://ourworldindata.org/trade-and-globalization |

## 备注

- World Bank / KOF 是"国家 × 年份"的面板数据，最适合做着色地图。
- UN Comtrade 是"出口国 → 进口国"的流向数据，适合做流向图（比如石油贸易）。
- 用 ISO3 国家代码（USA, CHN…）作为统一键，方便和地图数据对接。
