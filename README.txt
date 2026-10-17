[1] 폰에 찬송가 폴더 복사
   PC의 D:\미가엘찬송가 폴더 전체(mp3, txt, list.csv)를 USB로 폰 저장공간에 복사
   (예: 내장 메모리/미가엘찬송가). mp3 3GB 정도라 몇 분 걸립니다.
   * SD카드/Download 폴더 등 어디든 가능. 단 Android 11 이상은 'Download' 폴더 최상위 자체는 선택 불가 -> 하위 폴더에 넣으세요.
   * 파일은 폴더 바로 아래에 있어야 합니다(하위 폴더 안은 읽지 않음).

[2] APK 만들기
   1. Android Studio 설치 (https://developer.android.com/studio)
   2. File > Open > HymnApp 폴더 선택 (처음엔 Gradle 동기화에 몇 분)
   3. Build > Build Bundle(s)/APK(s) > Build APK(s)
   4. locate 클릭 -> app-debug.apk (app/build/outputs/apk/debug/)
   5. 폰에 복사해 설치 ('출처를 알 수 없는 앱 설치' 허용)

[3] 앱 처음 실행
   폴더 선택 화면이 뜨면 복사해 둔 찬송가 폴더 선택 -> '이 폴더 사용' -> 허용.
   한 번만 하면 기억합니다. 폴더 변경은 상단 '폴더' 버튼.

[Android Studio 없이 APK 받는 방법 - GitHub 사용]
1. github.com 가입 후 New repository 생성 (Private 가능)
2. 이 폴더의 모든 파일(.github 폴더 포함)을 저장소에 업로드
   (Add file > Upload files, 숨김 폴더 .github 도 같이 끌어다 놓기)
3. 저장소의 Actions 탭 > Build APK > Run workflow
4. 3~5분 뒤 완료되면 해당 실행 화면 아래 Artifacts 의 MikaelHymn-apk 다운로드 (zip 안에 app-debug.apk)
