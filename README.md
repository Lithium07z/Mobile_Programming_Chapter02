# 모바일 프로그래밍 · Android 입문 실습

2023년 2학기 모바일 프로그래밍 수업에서 작성한 Android·Kotlin 기초 실습입니다. XML로 화면을 구성하고, Kotlin 코드에서 버튼 클릭에 따라 화면의 텍스트를 바꾸는 과정을 다룹니다.

## 실습 내용

| 위치 | 내용 |
| --- | --- |
| [app](app) | `TextView`, `Button`, `ImageView`를 배치한 Android 앱 |
| [MainActivity.kt](app/src/main/java/com/example/androidlab/MainActivity.kt) | 두 버튼의 클릭 이벤트를 연결해 학번 또는 이름 표시 |
| [activity_main.xml](app/src/main/res/layout/activity_main.xml) | `ConstraintLayout`을 사용한 화면 배치 |
| [HelloWorld.kt](Lib3/src/main/java/com/example/lib3/Chapter3/HelloWorld.kt) | Android 화면과 별개로 실행하는 Kotlin 콘솔 예제 |

## 개발 환경

저장소의 Gradle 설정 기준입니다.

- Kotlin 1.8.0, Android Gradle Plugin 8.1.0, Gradle Wrapper 8.0
- Android SDK: `compileSdk` / `targetSdk` 33, `minSdk` 22
- `app` 모듈: Java / Kotlin JVM 대상 17
- Android Views(XML), AndroidX AppCompat, Material Components

## 실행 방법

1. 저장소를 복제하고 Android Studio에서 루트 폴더를 엽니다.
2. Gradle JDK를 17로 설정하고 Android SDK 33을 설치한 뒤 Gradle 동기화를 실행합니다.
3. 실행 모듈로 `app`을 선택하고 API 22 이상 에뮬레이터 또는 Android 기기에서 실행합니다.
4. 화면의 두 버튼을 눌러 중앙 텍스트가 바뀌는지 확인합니다.

`Lib3`의 콘솔 예제는 `HelloWorld.kt`의 `main()` 옆 실행 버튼으로 개별 실행합니다. 이 JVM 라이브러리 모듈은 Java 대상 버전이 1.7이고 Kotlin의 `jvmTarget`은 별도 지정하지 않았습니다. Gradle이 JVM 대상 불일치를 보고하면 모듈의 Java·Kotlin 대상 버전을 맞춰야 합니다.

## 참고

수업 당시 코드를 보존한 학습용 저장소입니다. 위 내용은 소스와 빌드 설정을 기준으로 정리했으며, 최신 Android Studio에서의 빌드·기기 실행은 별도 검증하지 않았습니다.
