> [!CAUTION]
>
> 이 문서는 오래된 문서입니다. 참고하지 마십시오.

<h2 id="목차">목차</h2>
현재 프로젝트는 두 가지 유형의 API 를 지원하며, 모든 방법에는 Redis 가 필요합니다;

- [Python 에서의 함수 호출](#api-python)
- [HTTP 프로토콜](#api-http)

---

<h2 id="api-python">Python</h2>

`pdf2zh` 는 Python 에 설치된 모듈이므로, 다른 프로그램에서 호출할 수 있는 두 가지 메소드를 Python 스크립트에서 제공합니다.

예를 들어, Google Translate 를 사용하여 영어 문서를 중국어로 번역하려면 다음 코드를 사용할 수 있습니다:

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
파일로 번역하기:
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
스트림으로 번역하기
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ 맨 위로 이동](#toc)

---

<h2 id="api-http">HTTP</h2>

보다 유연한 방법으로, 다음과 같은 경우 HTTP 프로토콜을 사용하여 프로그램과 통신할 수 있습니다:

1. 백엔드 설치 및 실행

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. 다음과 같이 HTTP 프로토콜 사용:

   - 번역 작업 제출

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - 진행 상태 확인

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - 진행 상태 확인 _(완료 시)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - 단일 언어 파일 저장

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - 이중 언어 파일 저장

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - 실행 중인 경우 중단하고 작업 삭제
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ 맨 위로 이동](#toc)

---

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>