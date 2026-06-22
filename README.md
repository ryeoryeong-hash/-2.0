# -2.0
# Cinderella-GPT 프로젝트 (nanoGPT 활용)

### 1. 프로젝트 목적
* nanoGPT 프레임워크를 활용하여 캐릭터 수준(character-level)의 GPT-2 기반 모델을 구현하고, 직접 작성한 신데렐라 동화 데이터셋을 학습시켜 텍스트 생성 능력을 평가함.

### 2. 학습 설정 및 결과
* **Dataset**: 신데렐라 동화 텍스트 (직접 작성)
* **Training**: 500 iterations, batch_size 64, block_size 256
* **Final Loss**: train loss 0.0200 달성

### 3. 주요 구성 파일
* `data/my_dataset/`: 데이터 전처리 파일 (`train.bin`, `val.bin`, `meta.pkl`)
* `out-my-dataset/ckpt.pt`: 학습 완료된 모델 체크포인트
* `Untitled5.ipynb`: 전체 학습 파이프라인(데이터 준비~생성) 코드

### 4. 생성 결과 샘플
* 입력: "옛날"
* 출력: "옛날, 왕궁으로 떠났습니다. 홀로 남은 신데렐라는 눈물을 흘렸습니다. “나도 한 번쯤 아름다운 옷을 입고 춤을 춰 보고 싶었는데….”..."
