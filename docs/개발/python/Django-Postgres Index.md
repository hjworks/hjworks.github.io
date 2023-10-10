# BloomIndex

* 
* Postgresql에 bloomIndex Extension을 설치해야 한다

# B-Tree
* Postgres 기본 인덱스
### 장점
* index row 의 `is_null`, `is_not_null` 등 처리할 때 속도가 매우 빠르다
### 단점
* 정렬이 되어 있어야 한다.

# Hash
* index row 에 `=` 를 사용할 때 성능이 빠르다

# GiST
* 다양한 인덱스 연산자를 수행할 수 있다.
# SP-GiST

# GIN
### 단점
* indexed key에 heap row 삽입 / 업데이트 시 느리다
* 디스크 많이 사용함

# BRIN
* 물리적인 블록 범위에 대한 요약본을 저장한다.
* 테이블 행이 물리적으로 근접해 있을 때 성능이 좋다.

# jsonb 필드를 가진 django model 에 최적의 인덱스는?
https://medium.com/@thegalang/indexing-in-postgresql-and-applying-it-to-jsonb-c99ecf50a443
### GIN
* 완전일치 검색 수행 시 GIN 이 최적이다.
### TRIGRAM
* 패턴매칭 검색에 최적이다(Pandas를 이용한) 데이터 분석 실습  : 2/e

### Hash
### BTree


### 다양한 키가 존재하는 단순 완전일치 검색에 대해서 GIN 성능 좋다
### 또는 BTree도 좋다.


