# [Workbook 1] Packages and Folders

## Overview

이 연습에서는 향후 Workbook 에서 수행할 Integration Server 내 개발 컴포넌트들을 저장할 Package 와 Folder 를 만듭니다.

 

## Steps


개발을 시작하기 위해서 개발 컴포넌트들을 보관할 Package 와 Folder 가 필요합니다.

#### STEP 1. IBM webMethods Designer 를 열고 기본 workspace을 유지한 다음 Use this as the default and do not ask again 옆의 상자를 선택합니다.

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled.png)

#### STEP 2. Designer 에서 IS 개발 환경 화면인 Service Development 화면을 엽니다.

- 메인화면의 Open the Service Development Perspective 를 클릭합니다.
![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/new2.png)


#### STEP 3. 서버 연결을 위해 Package Navigator 우측 상단에서 Add or modifiy Integration Severs를 선택 후 연결 정보를 입력합니다. 

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/167b22ea-9c09-4378-bb90-dc947074fcd2.png)

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled1.png)


- 접속정보 
  - Name : 디자이너에서 접속할 IS 서버의 별칭 지정 (ex. IS_74)
  - Host: 211.238.108.74
  - Port : 5555
  - User : 제공된 계정
  - Password: 제공된 계정


#### STEP 4. 본 연습에서는 제공된 EDUxxxx 계정을 사용해서 패키지를 생성합니다. (ex. EDU0000) 

- 패키지는 Package Navigator 에서 우클릭 New > Package 를 클릭하여 생성 할 수 있습니다.

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled%204.png)

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled5.png)

**Note.** Package 와 Folder의 네이밍 룰은 고객사 별로 상이하게 관리하며, 일반적으로 IFID을 포함하여 생성합니다. (ex. IFID_소스시스템명_타겟시스템명)   

#### STEP 5. 생성 된 package에서 제공된 계정 동일한 명칭의 Folder를 만듭니다.

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled%206.png)

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled7.png)

**Note.** Integration Server 는 Folder 구조에 의해 컴포넌트들이 고유하게 식별되므로 Package 바로 하위 폴더는 Package 명과 동일하게 구성할 것을 권장 드립니다. (Namespace 충돌 방지)

#### STEP 6. 생성 된 하위폴더에 IF0001이라는 폴더를 만듭니다.

#### STEP 7. IF0001 폴더에 다음과 같은 6개의 폴더를 생성합니다.
 - adpt (Adapter Service용 폴더 예시)
 - docs (Document Type용 폴더 예시)
 - noti (Notification용 폴더 예시)
 - ws (WebService용 폴더 예시)
 - api (REST API용 폴더 예시)
 - svc (Flow Service용 폴더 예시)

![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled8.png)

**참고:** 이 폴더들을 모두 정확한 위치에 놓으려면 매번 폴더를 생성할 상위 폴더에 마우스 오른쪽 단추로 클릭하고 New -> Folder를 선택합니다. 만약 이름을 잘못 입력한 경우에는 마우스 오른쪽 단추로 클릭하고 Rename을 선택합니다.

#### STEP 8. IF0001.ws 와 IF0001.api 폴더에서는 다음과 같은 하위 폴더 두개를 새로 만듭니다.
 - **consumer (Consumer 용** **폴더)**
 - **provider (Provider 용** **폴더)**

   ![Untitled](%5BWorkbook%201%5D%20Packages%20and%20Folders%2056c093055c3c4316823cf3b81439a900/Untitled%209.png)

   


