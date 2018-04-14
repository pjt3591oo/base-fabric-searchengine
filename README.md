# search engine

Crawler is bot that scraping on website from search engine and etc site.

Collected datas saved blockchain(Hyperledger fabric).

# database

* elasticsearch
  * 형태소 분석
  * for Hyperledger Fabric process killed

* Hyperledger fabric
  * Keyword - Address mapping saved
  * Keyword search Count
  * Address search Count

# Datastruct

```text
키워드 {
  검색횟수
  주소리스트
}

주소 {
  방문횟수
  키워드
}
```

```go
type Keyword struct {
  Count int
  Address []string
}

type Address struct {
  Count int
  Address []string
}

```

# Invoke

* saved - keyword and address mapping infos save from crawler
* searched - keyword count
* visited - address count

# Query

* 키워드 검색 후 키워드에 매핑된 주소 리스트 뿌려주기
