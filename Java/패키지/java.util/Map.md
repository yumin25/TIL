## Map
key : 중복 x
value : 중복 O
<br>dictionary와 비슷. 순서 x

<br>

선언
```java
import java.util.HashMap;

HashMap<String, String> map = new HashMap<String, String>();
```
new에서 타입 파라미터 생략 가능<br>
new에서 초기 용량 지정  ex) new HashMap<>(10);

<br>


* put : 값 추가
```java
map.put("key1", "value1");
```

<br>

* remove : 값 제거
```java
map.remove("key1");
```

<br>

* get : key에 해당하는 value값 가져오기
```java
map.get("key1");
```

<br>

* containsKey : map에 해당 key 유무 조사 후 결과값 리턴
```java
map.containsKey("key1");
```

<br>

* containsValue : map에 해당 value 유무 조사 후 결과값 리턴
```java
map.containsValue("value1");
```

<br>

* size : map의 갯수 리턴
```java
map.size();
```

<br>

* clear : 모든 값 제거
```java
map.clear();
```

<br>

* keySet : key값 출력
```java
Set<String> keys = map.keySet();
```

이용해서 전체 값 출력

```java
for (String key : map.keySet()) {
			System.out.println("key = " + key + ", value = " + map.get(key));
		}
```
<br>

* entrySet : hashmap에 저장된 key-value 값을 엔트리 형태로 set에 저장해 반환
```java
Set<Entry<String, String>> entrySet = map.entrySet();
```

이용해서 전체 값 출력

```java
for (Map.Entry<String, String> entry : map.entrySet()) {
			System.out.println("key = " + entry.getKey() + ", value = " + entry.getValue());
		}

```
<br><br>

LinkedHashMap : 입력된 순서대로 data 정렬<br>
TreeMap : 이진 검색 트리 형태로 저장. 키값에 따라 오름차순으로 data 정렬