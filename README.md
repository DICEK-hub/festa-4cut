# FESTA 4CUT — GitHub Pages

학교 축제 포토부스 정식 v1.0.0의 정적 배포 전용 저장소입니다.

배포 주소: https://dicek-hub.github.io/festa-4cut/

승인된 앱 소스 커밋: b010d8206299db1356fcef91a78f8357af6e18c3 (v1.0.0). 배포 저장소의 커밋과 앱 소스 커밋은 구분합니다. build-info.json에 앱 출처, 필터/테스트 설정, 빌드 자산 해시가 기록되어 있습니다. 소스 전체·내부 문서·연구 자료·인증 정보는 이 저장소에 넣지 않습니다. 이미지 자산은 승인된 생성 샘플과 프레임입니다. 실제 학생 사진은 업로드하지 않습니다.

GitHub Settings → Pages → Build and deployment → Deploy from a branch, main / (root). .nojekyll로 정적 파일을 그대로 게시합니다. JavaScript/CSS/이미지의 Vite base는 /festa-4cut/입니다. 필터는 활성화하고 테스트 진입은 숨깁니다. 폰트는 시스템 폰트를 사용하고 아이콘은 앱 번들에 포함됩니다. 기존 ChatGPT Sites 배포 설정과 분리되어 있습니다.

## 업데이트

1. 승인된 소스 커밋/태그를 별도 작업 폴더로 추출합니다. 최신 개발 브랜치를 자동 사용하지 않습니다.
2. 기존 pnpm build 및 전체 자동 테스트를 실행합니다.
3. GitHub Pages 전용 Vite 설정에서 base /festa-4cut/, VITE_ENABLE_PHOTO_FILTERS=true, VITE_ENABLE_TEST_MODE=false, sourcemap=false를 지정해 빌드합니다. ChatGPT Sites 설정은 바꾸지 않습니다.
4. 검사한 정적 결과와 build-info.json만 이 배포 저장소에 반영합니다. 소스·.env·인증정보·사진·연구 자료는 복사하지 않습니다.
5. 사용자 승인 범위 안에서 새 커밋을 만들고 main에 일반 push합니다. 이 저장소의 main push는 Pages 재배포를 시작합니다. 기존 개발 저장소의 push는 이 사이트에 자동 반영되지 않습니다.
6. Pages 빌드 완료와 실제 HTTPS 자산/20가지 프레임·필터 조합을 확인합니다. iPad 카메라 권한·사진 저장·단축어·프린터 출력은 새 주소에서 별도 확인합니다.

## 복구

문제 배포를 새 revert 커밋으로 취소해 일반 push하거나, 승인된 이전 정적 결과를 새 커밋으로 다시 배포합니다. 강제 push나 이력 재작성을 하지 않습니다. 기존 https://festa-4cut.hougub.chatgpt.site/ 운영 사이트는 별도로 유지됩니다.
