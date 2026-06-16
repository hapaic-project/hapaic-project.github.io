## 저장소에 대한 설명

|저장소 이름|설명|
|:--:|:--|
|hapaic-project.github.io|프로젝트 소개 페이지|
|== vLLM ==||
|vllm-uneven|비균등 분할 텐서 병렬화 프로토타입|
|vllm-plus| |
|==tenstorrent ==||
|tt-metal||
|kmd||
|umd||
|==plugin==||
|vllm-tt||
|vllm-tt-plugin-rdma||
|vllm-tt-prefill||
|vllm-tt-decode||
|tt-inference-server|내부 개발용|
|tt-inference-server-fork|PR 요청용 tt-inference-server|
|==KV Cache Mgmt==||
|tt-LMCache|  |
|mooncake-transfer-engine||
|==Benchmark & Demo==||
|vLLM-Benchmark-dataset|벤치마크 데이터 셑|
|demo-repository|데모|

## vLLM V0-Based GPU–NPU Disaggregated Prefill(w/RDMA)
| 구성요소 | version | 저장소 | branch |
| --- | --- | --- | --- |
| tt-metal (NPU) | v0.65 | https://github.com/hapaic-project/tt-metal | `dev-0.65` |
| umd (NPU) | v0.65 | https://github.com/hapaic-project/tt-umd | `dev-0.65` |
| kmd (NPU) | v2.5.0 | https://github.com/hapaic-project/tt-kmd | `dev-v2.5.0` |
| vllm_v0_tt_plugin (NPU) | v0.10.0 base | https://github.com/hapaic-project/vllm_v0_tt_plugin ||
| vllm_v0_decode (NPU) | v0.10.0 base | https://github.com/hapaic-project/vllm_v0_decode ||
| vllm_v0_prefill (GPU) | v0.10.0 base | https://github.com/hapaic-project/vllm_v0_prefill ||
| mooncake-transfer-engine (NPU, GPU) | v0.3.6 | https://github.com/hapaic-project/mooncake-transfer-engine | `main` |

## vLLM V1-Based GPU–NPU Disaggregated Prefill(w/RDMA)
*작성 기준(2026.6.15) single request만 가능
| 구성요소 | version | 저장소 | branch |
| --- | --- | --- | --- |
| tt-metal (NPU) | v0.68 | https://github.com/hapaic-project/tt-metal | `dev-0.68` |
| umd (NPU) | v0.68 | https://github.com/hapaic-project/tt-umd | `dev-0.68` |
| kmd (NPU) | v2.5.0 | https://github.com/hapaic-project/tt-kmd | `dev-v2.5.0` |
| tt-inference-server (NPU) | v0.18.1 base | https://github.com/hapaic-project/tt-inference-server | `v0.2_rdma_single` |
| vllm-plus (NPU, GPU) | v0.18.1 base | https://github.com/hapaic-project/vllm-plus | `gpt2tt_rdma_dev` |
| mooncake-transfer-engine (NPU, GPU) | v0.3.9 | 수정  x) pip install로 설치함 | - |
