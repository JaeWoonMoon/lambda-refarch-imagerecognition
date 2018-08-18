# Hands-On : Amazon Rekognition를 이용한 이미지 인식 태깅 서비스 만들기

이 핸즈온에서는 AWS Step Functions를 사용하여 서버리스 이미지 인식 프로세싱 워크 플로우를 단계별로 구축하는 방법을 배우게됩니다.

아래 다이어그램에서 볼 수 있듯이 워크플로는 Amazon S3에 업로드 된 사진을 처리하여 위치 정보, 크기/형식, 시간 등과 같은 메타 데이터를 이미지에서 추출합니다. 그런 다음 Amazon Rekognition을 사용하여 사진의 객체에 태그를 지정합니다. 동시에, 웹앱에서 사용할 썸네일 이미지를 생성합니다. AWS Step Functions은 다양한 단계를 조정하기 위해 오케스트레이션 역할을합니다.

![상태 시스템에 대한 IAM 역할 선택](../images/photo-processing-backend-diagram.png)

## 준비물

- AWS 계정에 대한 관리 액세스
- 자신 손에 익은 코드 편집기 (예 : Sublime Text, PyCharm 등)

## 지침

* [단계 0: 리소스 설정](step-0.md)
* [단계 1: AWS Step Functions 상태 머신에 첫 번째 람다 단계 추가](step-1.md)
* [단계 2: 상태 머신에 분기 로직 추가](step-2.md)
* [단계 3: 워크 플로우에 병렬 처리 추가](step-3.md)
* [단계 4: 레이블 및 이미지 메타 데이터 유지](step-4.md)
* [단계 5: S3 이벤트 실행 시작](step-5.md)
* [단계 6: 웹 응용 프로그램 빌드 및 실행](step-6.md)
* [추가 옵션](additional-steps.md)
* [자원 정리](clean-up.md)
