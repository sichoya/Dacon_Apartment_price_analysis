이 데이터는 데이콘의 해당 대회의 대회안내 - 동의사항에 따라 공유를 일부 제한합니다.
불러오는 코드 또한 마찬가지입니다.

url : https://dacon.io/competitions/official/236130/data

1. train.csv
        id : 구분자(ID)
        sigungu : 아파트의 지역
        jibun : 지번
        apt_name : 아파트 이름
        exclusive_use_area : 소유자가 독점적으로 사용할 수 있는 공간
        transaction_year_month : 거래 연월
        transaction_day : 거래일자
        transaction_real_price : 실 거래 가격(TARGET)
        floor : 층수
        year_of_completion : 건설 완료 연도

2. test.csv
        id : 구분자(ID)
        sigungu : 아파트의 지역
        jibun : 지번
        apt_name : 아파트 이름
        exclusive_use_area : 소유자가 독점적으로 사용할 수 있는 공간
        transaction_year_month : 거래 연월
        transaction_day : 거래일자
        floor : 층수
        year_of_completion : 건설 완료 연도

3. submission.csv
        id : 구분자(ID)
        transaction_real_price : 실 거래 가격(TARGET)



```python\
train = train[['exclusive_use_area', 'transaction_year_month', 'floor', 'year_of_completion', 'transaction_real_price']]\
test = test[['exclusive_use_area', 'transaction_year_month', 'floor', 'year_of_completion']]\
```\
\
```python\
train_x = train.drop('transaction_real_price', 
\f2\i axis
\f0\i0 =1)\
train_y = train['transaction_real_price']\
```}
