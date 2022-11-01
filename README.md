# folder-tree
New Project Folder Tree     
신규 프로젝트 진행 시 폴더 트리 구성하기    
-----

개발자마다, 회사마다 폴더를 생성하고 구조를 만드는 것은 모두 조금씩 다르겠지만     
나는 내나름의 기준을 세우고 어떤 프로젝트를 하더라도 버벅거리지 않고 뚝딱 뚝딱 만들고싶었다.      
그래서 정리해보기~~~    

회사에서의 경우 한 저장소에 많~~은 서비스가 들어가 있는 경우에는 폴더명으로 많이 세분화 시키겠지만    
일단 개인프로젝트 중 한가지 프로젝트를 위해 폴더트리를 생성할 경우! 라고 가정하고 만들어보았습니다.

홈페이지가 반응형일 때 / PC와 Mobile로 나누어져 있을 때 / 서비스가 한 저장소에 많이 있을 때    
모두 조금씩 다르겠지만, 기본적인 구조는 똑같다고 생각한다.

### Tree
```
📦project
 ┗ 📂src
 ┃ ┣ 📂html
 ┃ ┃ ┣ 📂include
 ┃ ┃ ┃ ┣ 📜_module1.html // 페이지에서 사용될 모듈
 ┃ ┃ ┃ ┗ 📜_module2.html
 ┃ ┃ ┣ 📜00_a.html // 페이지
 ┃ ┃ ┗ 📜01_b.html
 ┃ ┣ 📂images // 이미지 폴더
 ┃ ┗ 📂scss
 ┃ ┃ ┣ 📂common
 ┃ ┃ ┃ ┣ 📜common.scss // 공통
 ┃ ┃ ┃ ┣ 📜layout.scss // 페이지 레이아웃
 ┃ ┃ ┃ ┣ 📜mixins.scss // mixin
 ┃ ┃ ┃ ┗ 📜variables.scss // 사용자 지정 변수
 ┃ ┃ ┣ 📂ui // 모듈별 스타일로 html>include 폴더에 있는 모듈과 파일명을 동일하게 하는게 좋다 
 ┃ ┃ ┃ ┣ 📜_module1.scss
 ┃ ┃ ┃ ┗ 📜_module2.scss
 ┃ ┃ ┗ 📜project.scss // 전체 스타일 파일 import
```