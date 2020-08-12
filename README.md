## 주식 투자 프로젝트
### FinanceDataReader
  - 국내, 해외 주식데이터를 Pandas 형태로 불러올 수 있는 Python Package
  - 설치법 및 튜토리얼은 다음 페이지를 참조
      - https://github.com/FinanceData/FinanceDataReader 

#### StockListing 
주식시장에 상장되어 있는 회사 정보를 조회하는 함수
 - 주식시장, 업종, 상장일시, 회사대표, 홈페이지 등의 정보를 조회하는 코드는 아래와 같다.
 
```python
import FinanceDataReader as fdr
krx = fdr.StockListing('KRX')
krx.head(10)
```
#### ETFListing
주식시장에서 거래되는  ETF 상품을 조회할 수 있는 함수

```python
#import FinanceDataReader as fdr
df_etf = fdr.EtfListing('KR')
df_etf.head(10)
```