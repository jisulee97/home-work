### HTML 코드 설명

- 가장 바깥쪽 상자를 section, 인기 사이트는 제목이기 때문에 h2로 주었고 사이트 부분이
색이 다르기 때문에 span 태그로 묶었다

- 리스트 스타일은 ol, li 태그를 사용하였고 각각의 항목에 a 링크를 넣었다

### css 코드 설명

- 각각의 간격들은 패딩과 마진으로 조정하였다

- site-list 부분은 display: flex/ justify-content: space-between 속성을 주어 양쪽으로
  배치하였다
- 각각의 리스트 앞에 숫자들은 ::before 으로 가상 요소를 만들어 디자인을 하였다
  display: inline-block 속성을 주어 줄바꿈이 일어나지 않도록 하였다

- sprite 클래스를 만들어 배경이미지로 넣은 후 각각의 li 에 sprite 클래스를 주어 이미지를
  삽입한 후 위치를 조정하였다

- third-list 부분은 배경 이미지가 완벽하게 가려지지 않아 li에 height를 주어 튀어나온
  부분을 가려주었다

