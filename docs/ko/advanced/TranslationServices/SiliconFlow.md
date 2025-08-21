# 실리콘플로우

## 무료 번역 서비스

[SiliconFlow](https://siliconflow.cn) 은 이 프로젝트를 위해 무료 번역 서비스를 제공합니다.

현재 무료 번역 서비스는 `THUDM/GLM-4-9B-0414` 모델을 사용합니다.

### 사용법

#### 명령줄

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### 웹 UI

1. "번역 옵션" - "서비스" 드롭다운 목록에서 "SiliconFlowFree"를 선택합니다.
2. 페이지 하단의 "번역" 버튼을 클릭하여 번역을 시작합니다.
3. 번역이 완료된 후, 페이지 하단의 "번역된 파일" 섹션에서 번역된 `PDF` 파일을 찾을 수 있습니다.


### 개인정보 처리방침

파일 내용은 프로젝트 관리자 [@awwaawwa](https://github.com/awwaawwa) 의 서버로 전송된 후 SiliconFlow 로 전달되어 번역됩니다.

이 프로젝트의 관리자들은 SiliconFlow 에서 반환된 오류 정보만을 수집하여 관련 서비스 디버깅에 사용합니다. 귀하의 파일 내용은 수집되지 않습니다.

SiliconFlow 개인정보 처리방침: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## SiliconFlow 에서 다른 모델 사용하기

[SiliconFlow](https://siliconflow.cn) 는 번역을 위한 다른 모델도 제공합니다.

### 사용법

1. [SiliconFlow](https://siliconflow.cn) 에서 계정을 등록하세요.

2. [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak) 에서 API 키를 생성하세요. 그런 다음 키를 클릭하여 복사하세요.

#### 명령줄

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### 웹 UI

1. "번역 옵션" - **"서비스"** 드롭다운 목록: "SiliconFlow" 선택
2. "번역 옵션" - **"SiliconFlow API 기본 URL"**: 기본값 유지
3. "번역 옵션" - **"사용할 SiliconFlow 모델"**: "Pro/deepseek-ai/DeepSeek-V3" 또는 다른 모델 입력
4. "번역 옵션" - **"SiliconFlow 서비스 API 키"**: API 키 붙여넣기
5. 페이지 하단의 번역 버튼을 클릭하여 번역 시작
6. 번역이 완료된 후, 페이지 하단의 "번역됨" 섹션에서 번역된 `PDF` 파일을 찾을 수 있습니다.


## 감사의 말

[SiliconFlow](https://siliconflow.cn) 에 이 프로젝트를 위한 무료 번역 서비스를 제공해 주셔서 감사합니다.

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>