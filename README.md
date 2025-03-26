**▶ 정적 크롤링과 동적 크롤링에 관하여**
1) **정적 크롤링**
   원리 : 한 URL 에서 원하는 항목을 전부 가져와서 리스트업 해놓는 방법
   추가설명 :
     원하는 항목 = 아래 그림처럼 원하는 크롤링 URL의 F12 버튼을 누르고 크롤링하고 싶은 부분을 클릭하면 해당 태그 (body, div, h3 등) 과 그 내부에 id(Class)가 담겨있는 것이 보일것이다.(아래 
     그림) 
     크롤링 방법 = 해당 항목을 soup = bs(reponse.text, "html.parser")와 같은 코드 설정 후 soup.find(해당 항목) 으로 모든 것을 담는다. 

![image](https://github.com/user-attachments/assets/9aef309c-d2d0-48b7-9777-67fbad6c26ad)

2) **동적 크롤링**
   원리 : chromedriver를 통해 원하는 항목을 찾아다니면서 크롤링 하는 방법 (단, 시작지점은 정적 크롤링과 같이 URL을 통해 시작한다.)

