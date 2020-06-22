# basic-cf-model: plyst_id를 user, song을 items로 보았을 때 간단 CF 모델 구현
# basic-cf-model-v2: basic-cf-model 코드 효율성 제고, val.json의 각 plyst 중, songs가 주어진 plyst에 100개의 곡을 추천한 pickle 파일 생성
  # cf_val_recommendation.pkl
  # results.json: 카카오 아레나에 제출하려고 만든 파일이나, 리더보드 제출 시 모든 plyst에 대한 100개의 곡 + 10개의 태그가 꼭 할당되어야해서 오류 뜸
    # 추후, songs가 주어지지 않은 plyst의 경우 best seller 모델이나, 다른 방법을 통해 추천 곡을 뽑아서 다시 results.json 파일 만들어야 함
    # tag 또한 마찬가지
# train-test-split-nDCG: 모델 성능 체크용으로 train.json에서 train/test set 분리 후, test set에서 일정부분 mask하여 가리는 함수, nDCG 계산 함수
