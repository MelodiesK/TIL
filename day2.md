# 2일차 정리

- 명령어

```
git init : 현재 작업중인 디렉토리를 깃으로 관리하기 시작한다는 명령어
git status : 깃의 현재상태을 알려주는 명령어
git add '파일이름': 깃의 작업공간에 파일을 추가해주는 명령어 (파일이 U 혹은 M에서 A로 변경됨)
git commit -m '메시지' : 파일의 변경상태를 저장하는 명령어 메시지는
					git log --oneline 명령어를 통해서 열람가능하므로 변경사항을 적어줄것
git log : 깃의 ID, 변경자, 시간, 메시지 등을 조회할수있는 명령어
			빠져나갈때는 Q버튼을 이용한다
			옵션으로 대략적으로 보고싶다면 git log --oneline 을통해 한줄로 축약해준다
git remote add "이름" "주소" : 주소에 있는 원격저장소를 저장위치로 삼겠다는 명령어
								저장시에 저장소 임의로 지정한 "이름"으로 저장위치 지정
git push "이름" master : "이름"에 업로드하여 저장 하겠다는 명령어
git clone "주소" "폴더이름" : "주소"에 있는 커밋내역을 내 컴퓨터로 가저오겠다는 명령어
					새폴더를 만들수 있으며 자동적으로 git init되어있다
					폴더이름은 생략가능하며 그럴시 그폴더에 클론을 만든다
git pull "이름" master : "이름"에 업로드된 로컬데이터와 원격저장소의 내용이 다를시
						원격 저장소의 내용을 당겨오는 명령어
						(완전히 일치시 아무일도 일어나지 않음)
```



- .gitignore

특정 파일 혹은 폴더에 대해 Git이 버전 관리를 하지 못하도록 지정하는 것

자동으로 생성되는 파일, 혹은 업로드를 원하지않는 작업결과를 자동적으로 배제하기 위해 사용되는 파일

1. touch .gitignore 를 통해 생성

2. 내용에 무시할 파일이름을 적용, 혹은 https://www.toptal.com/developers/gitignore 를 통해 자신의 상황에 맞는 gitignore 를 만들어 적용
3. 원격저장소에 업로드시 git에 적용됨





