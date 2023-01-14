# 템플릿

## 가장 중요한 것
![img.png](img.png)

### 트랜잭션의 경계 설정
- 트랜잭션이 시작되고 끝나는 위치
  - 해당 위치 설정 작업은 매우 중요하다.
- 트랜잭션의 시작과 종료는 Connection을 통해 이뤄진다. 
  - autoCommit = false로 설정해주면 트랜잭션 시작 
- 하나의 DB 커넥션 안에서 만들어지는 트랜잭션 -> 로컬 트랜잭션 

## 중요한 것
```java
TransactionSynchronizationManager.initSynchronization();  // 트랜잭션 동기화 매니저
DataSourceUtils.getConnection(dataSource);
```

## 궁금한 것 
### 쓰레드 로컬이 어떻게 동작하는지 알아보자 