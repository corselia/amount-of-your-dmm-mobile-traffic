[![CircleCI](https://circleci.com/gh/corselia/amount-of-your-dmm-mobile-traffic.svg?style=svg)](https://circleci.com/gh/corselia/amount-of-your-dmm-mobile-traffic)

# DMMモバイルのマイページ内の「データ通信量照会」のデータを取得する

![データ通信量照会_01](docs/dmm_mobile_data_traffic_info_table_01.png "データ通信量照会_01")

![データ通信量照会_02](docs/dmm_mobile_data_traffic_info_table_02.png "データ通信量照会_02")

## HTML の構造

### 電話番号 の部分
- 1つ目の電話番号
  - `#fn-number > option:nth-child(1)`
- 2つ目の電話番号
  - `#fn-number > option:nth-child(2)`
- 3つ目の電話番号
  - `#fn-number > option:nth-child(3)`

### 料金表 の部分

#### thead の部分
- 日付
  - `body > section > div > section.area-right > section.box-recentCharge > div > table > thead > tr > th:nth-child(1)`
- 高速データ通信量
  - `body > section > div > section.area-right > section.box-recentCharge > div > table > thead > tr > th:nth-child(2)`
- 低速データ通信量
  - `body > section > div > section.area-right > section.box-recentCharge > div > table > thead > tr > th:nth-child(3)`
- SNSフリー通信量
  - `body > section > div > section.area-right > section.box-recentCharge > div > table > thead > tr > th:nth-child(4)`

#### tbody の部分

##### 1行目（最初の行） の部分
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(1) > td:nth-child(1)`
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(1) > td:nth-child(2)`
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(1) > td:nth-child(3)`
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(1) > td:nth-child(4)`

##### 30行目（最後の行） の部分
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(30) > td:nth-child(1)`
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(30) > td:nth-child(2)`
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(30) > td:nth-child(3)`
- `body > section > div > section.area-right > section.box-recentCharge > div > table > tbody > tr:nth-child(30) > td:nth-child(4)`
