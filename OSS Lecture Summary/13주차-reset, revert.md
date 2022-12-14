# 되돌리기
깃에서 코드 작업을 되돌리는 방법에는 2개가 있다.

## 📌 reset
✔️ 커밋을 기준으로 이전 코드로 되돌리는 방법으로, 기록한 커밋을 취소한다.
<br/>

```bash
git reset 옵션 커밋ID
```

위와 같이 reset 명령어를 사용하면 지정된 커밋 코드로 되돌아간다. 옵션은 다음과 같이 총 3가지가 있다.

- **soft** : 스테이지 영역을 포함한 상태로 복원한다.  
- **mixed** : 기본 옵션 값은 mixed임. reset 명령어를 사용할 때 옵션을 지정하지 않으면 기본값인 mixed로 선택된다.  
- **hard** : 실제 파일이 삭제된 이전 상태로 복원한다.
<br/><br/>

## :pushpin: revert
✔️ 기존 커밋 정보를 삭제하는 리셋과 달리 리버트는 기존 커밋을 남겨 두고 취소에 대한 새로운 커밋을 생성한다.   
✔️ 리버트는 한 번에 커밋 하나만 취소할 수 있다.
<br/>

```bash
git revert 커밋 ID
```

위와 같이 커밋 해시 값을 지정하여 특정 커밋을 취소할 수 있다. 바로 이전 커밋을 취소하기 위해서는 커밋 ID 대신에 'HEAD'를 적어줄 수 있다.
<br/>


```bash
git revert 커밋 ID .. 커밋 ID
```

위와 같이 깃의 범위 지정 연산자를 사용해 여러 커밋을 리버트할 수도 있다.
