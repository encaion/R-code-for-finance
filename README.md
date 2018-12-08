# R-code-for-finance
R code for finance <br>
주식, 재무표, 데이터를 위해 만든 repo입니다. 

# 2018.12.08 UPDATE
1. 마감시황 업데이트 되었습니다<br>
- 주말에 금요일 시황이 뜨지 않던 에러를 수정하였습니다.<br>
<br>
2. KRX종목테이블 항목이 추가되었습니다.<br>
- 코스피,코스닥,코스넥 종목을 회사명,종목코드, 업종 등으로 나누도록 하였습니다.<br>
- 종목코드는 6자리를 따릅니다. 예) 005930<br>
- function 사용법은 아래 '코드이용방법'을 참고해 주시기 바랍니다.<br>
<br>
3. 기존에 KRX데이터 때문에 실행이 불가능 했던 코드들을 수정하였습니다.<br>
- 재무제표 코드와 k-score 코드가 실행가능 한 상태로 되었습니다. 
<br>
4. 현재 홍콩주식은 사용이 불가한 상태입니다. 하루 빨리 수정하도록 하겠습니다.

# 2018.12.05 UPDATE
1. 마감시황 업데이트 되었습니다<br>
- DATE인식이 안되어서, 마감시황을 이용할 수 없다는 에러를 수정하였습니다.<br>
- 12월 5일 부시 전 대통령의 장례식으로 인한 갑작스러운 미국휴장에 코드가 시황을 인식하지 못하는 에러를 수정하였습니다.<br>
- 미국 뿐만 아니라 다른 나라 또한 예기치 못한 휴장을 방지하기 위해 코드를 수정하였습니다. 


# 코드 이용방법
- 홍콩주식과 중국주식은 홍콩재무제표, 중국재무제표를 나타냅니다. <br>
- 홍콩주식과 중국주식내 주식코드 테이블은 그냥 참고용이지, function과는 독립적이므로 원치 않으신 분들은 function만 import해도 됩니다. <br>
- 중국주식 이용방법 : cn_fs('코드번호') ex) cn_fs('000002') <br>
- 재무재표는 한국재무재표를 나타냅니다. 이용방법 kr_fs('기업명'), ex) kr_fs('삼성전자')
- SUPERTREND는 '코스닥종목'에 사용하지 않은 것을 추천합니다. 야후 파이낸스를 기반으로 데이터를 불러 오는데, 코스닥 종목은 누락된 데이터가 너무 많아 정확한 계산도출이 되지 않습니다. 추후에 한국주식 데이터베이스를 추가하도록 하겠습니다. 
- KRX종목 테이블 사용법 : 콘솔창에 KRX_data(save_csv_file=TRUE)로 입력하시면 기본 디렉토리에 'KRX테이블'이라는 엑셀파일이 csv 형식으로 저장됩니다. KRX_data() 혹은 KRX_data(FALSE)로 입력하실 경우, csv파일이 저장되지 않고 테이블로 뜨도록 하였습니다. 
