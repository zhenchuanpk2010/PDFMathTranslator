<!-- CHUNK ID: chunk_5BD35ED9  CHUNK TYPE: header START_LINE:1 -->
# Aliyun Qwen

<!-- CHUNK ID: chunk_ED2346E0  CHUNK TYPE: paragraph START_LINE:3 -->
It is recommended to use the `qwen-plus-latest` model.

Reference configuration:

<!-- CHUNK ID: chunk_B142B723  CHUNK TYPE: list START_LINE:7 -->
- Translation Service: `qwen-plus-latest`
- Base URL: keep default
- API key: your API key
- Timeout (seconds): 500
- Temperature: 0.0
- Send temperature: True
- Enable JSON mode: True

<!-- CHUNK ID: chunk_BC8076A9  CHUNK TYPE: paragraph START_LINE:15 -->
For rate limiting, use Custom mode:
<!-- CHUNK ID: chunk_7C20EF8C  CHUNK TYPE: list START_LINE:16 -->
- QPS: 30 or 40
- Pool Max Workers: 1000