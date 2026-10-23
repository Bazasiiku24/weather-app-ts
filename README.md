# Weather App

都市名から現在の天気を検索できるWebアプリです。

**公開URL**: https://weather-app-ts-kohl.vercel.app（Vercelの固定URL）

## 機能

- 都市名（英語）で検索して、気温・体感温度・湿度・風速・風向き・天気を表示

## 使用技術

- TypeScript / Vite
- Open-Meteo API（Geocoding API、Forecast API）
- Font Awesome

## 工夫した点

- 天気コードの対応表をオブジェクトにして、表示の処理を1か所にまとめた
- `response.ok`の確認と`try / catch / finally`で、通信失敗時もローディングが残らないようにした）
- APIの返り値に`interface`を定義して、`any`を使わないようにした
- Enter押しても機能するような直感的な操作を追加

## 既知の制限

- 漢字の地名が検索できない件。
- mediaによるレスポンス対応がない件。

## 開発方法

```bash
npm install
npm run dev
```
