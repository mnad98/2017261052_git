<h1>Git 명령어 정리</h1>
<h2>2017261052
 2반 장미나 </h2>
<h3>기본적인 명령어</h3> 
<p>git init :현재 디렉토리에</p> 
<p>git 저장소를 생성</p>
<p>git config —global —list :현재 설정정보 조회(--global옵션은 전역설정에 대한 옵션이여서 현재 프로젝트에만 적용할 때는 사용안함)</p> 
git config user.name :사용자명을 등록 (필수)
git config user.email :이메일 주소를 등록 (필수)
git —viersion :현재 git의 버전을 확인 
git add :git 저장소를 만들고 파일을 관리
git commit –m :스테이징 영역에 올라가 있는 파일들을 커밋. -m은 커밋메시지를 주는 옵션
git status :커밋되지 않은 변경사항을 조회
git diff :스테이징영역과 현재 작업트리의 차이점을 보여줌
git mv 파일명 새 파일명 :기존에 존재하는 파일을 새 파일로 이동
git checkout —파일명 :아직 스테이징이나 커밋을 하지 않은 파일의 변경내용을 취소하고 이전 커밋상태로 돌림

<h3>로그 관리</h3>
git log :커밋 로그들을 볼수 있음
git log 커밋명 :해당 커밋명의 로그를 볼 수 있음
git blame 파일명 :커밋명과 커밋한 사람들의 정보를 볼 수 있음
git revert 커밋명 :기존의 커밋에서 변경한 내용을 취소해서 새로운 커밋을 만듬
git reset 커밋명 :이전 커밋을 수정하기 위해서 사용

<h3>원격저장소</h3>
git clone 저장주소 폴더명 :원격저장소를 복제하여 저장소를 생성(폴더명 생략 가능)
git fetch :원격저장소의 변경사항을 가져와서 원격브랜치를 갱신
git remote add 이름 저장주소 :새로운 원격 저장소를 추가
git remote :추가한 원격저장소의 목록 확인
git remote show 이름 :해당 원격저장소의 정보를 볼 수 있음
git remote rm 이름 :원격저장소를 제거 

<h3>서브모듈</h3>
git submodule :연관된 하위모듈을 확인
git submodule add 저장주소 서브모듈경로 :새로운 하위모듈을 해당경로에 추가
git submodule init 서브모듈경로 :서브모듈을 초기화
git submodule update 서브모듈경로 :서브모듈의 변경사항을 적용
