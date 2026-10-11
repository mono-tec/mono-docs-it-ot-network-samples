# IT/OT Network Sample Docs

小規模企業向けIT/OTネットワーク構成を題材にした
サンプル設計資料です。

実案件の構成を公開するものではなく、
ネットワーク機器選定、VLAN、VPN、Wi-Fi、NAS、
セキュリティ、保守性などを検討するためのサンプルとして作成しています。

DXF等の編集用原本は公開せず、
公開資料はPDF形式のみとしています。

---

## 公開資料

本リポジトリでは、ITネットワークとOTネットワークを分けて
サンプル資料を管理します。

### IT-NETGEAR

NETGEAR製ネットワーク機器とFortiGateを使用した、
小規模企業向けITネットワーク構成サンプルです。

主な資料：

- 概算予算表
- 施設配置図
- ネットワーク構成図
- 機器一覧
- IPアドレス一覧
- ACL / Firewall Policy一覧
- Port図
  - FortiGate
  - Root Switch
  - Branch Switch
- 基本仕様書
- セキュリティ運用イメージ図
- 図面・資料一覧

一式をまとめたPDFと、
各資料を個別に分けたPDFを公開しています。

### OT-MOXA

MOXA製ネットワーク機器を使用した、
OT / FAネットワーク構成サンプルを格納する予定です。

※現在作成予定

---

## 想定するITネットワーク構成

IT-NETGEARサンプルでは、
主に以下の構成要素を想定しています。

- FortiGate
- Root Switch
- Branch Switch
- Edge Switch
- Wi-Fi AP
- NAS / Server
- VLAN
- VPN
- Guest Wi-Fi
- IoT Network

用途ごとにVLANおよびIPセグメントを分離し、
VLAN間通信はFortiGateで制御する構成を基本としています。

---

## セキュリティ・運用

サンプルでは、ネットワーク構成だけでなく、
以下のような運用についても扱います。

- VLANによる論理分離
- Firewall Policy / ACL
- VPN接続範囲の制限
- Guest Wi-Fiの分離
- IoTネットワークの分離
- FortiGateのFirmware / Security Patch運用
- Access Log / VPN Log / Security Logの確認
- 通信量の定期確認
- ログの長期保管・証拠保全
- 必要に応じた不審IP等の遮断

---

## 注意事項

本資料はサンプルです。

実際のネットワーク設計では、以下の条件に応じて
構成・機器・IPアドレス・VLAN・Firewall Policy・配線等を
調整する必要があります。

- 利用人数
- 建物構成
- 配線距離
- Internet回線
- 通信量
- セキュリティ要件
- 使用するクラウドサービス
- VPN利用範囲
- NAS / Server利用量
- IoT機器
- 可用性要件
- 将来増設

本資料に記載している機器構成、価格、設定例等は
実環境への適用を保証するものではありません。

DXF、Markdown等の編集用原本は公開していません。
公開資料はPDF形式のみです。

---

## Repository

```text
mono-docs-it-ot-network-samples/
├─ README.md
├─ IT-NETGEAR/
│  ├─ IT_OTネットワーク_サンプル.pdf
│  └─ docs/
└─ OT-MOXA/
   └─ docs/