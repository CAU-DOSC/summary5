# CathedralAndBazaarOrgByEsr

## 도입부
페치메일은 리눅스가 이룩한 새로운 소프트웨어 공학 이론을 검증하기 위해 만들어진 프로젝트이다. 저자는 이 프로젝트를 분석하는데 있어 상업용 소프트웨어를 의미하는 성당 모델과 반대로 리눅스 세계를 의미하는 시장 모델을 이용한다.
충분히 많은 사람이 있다면 찾을 수 없는 버그는 없다는 주장을 바탕으로 소프트웨어의 미래에 있어 이 통찰의 의미를 탐구해본다

## 성장과 시장
"리눅스는 파괴적이다."
과거 인터넷으로만 연결된 개발자에 의한 운영체제가 만들어지리라고는 상상조차 못했었다.
리눅스는 일반적인 많은 부분을 뒤집어 버렸다.
이전에는 소프트웨어는 몇 명의 도사 프로그래머나 작은 모임의 뛰어난 프로그래머에 의해 조심스럽게 만들고, 베타판도 없어야 한다고 여겨졌다.
그에비해 리눅스의 방식은 '자주 발표하며 다른 사람에게 위임할 수 있는 것을 모두 위임하고, 뒤범벅된 부분까지 공개하는' 방식이었다.
리눅스의 시장 방식이 효과적이라는 사실이 충격적이었다. 개개의 프로젝트에 열중했을 뿐아니라 리눅스 세계가 공중분해 되지 않고 이른바 성당 건축가들이 상상하기도 힘든 속도로 계속해서 강해지는지에 대한 부분이.
뒤의 이야기들은 효과적인 오픈소스 개발에 대한 격언을 제시할 것이다.

## 메일은 배달되어야만 한다
펜실베니아 주에 있는 조그만 무료 ISP업체에서 일하던 저자는 메일을 하나하나 확인하고 도착한 메일을 컴퓨터 도구를 이용해 다루고자 했지만 당시 프로그램 중에는 저자의 요구사항을 만족시킬 프로그램이 존재하지 않았다.
저자는 POP3 클라이언트가 필요했고 처음부터 모두 개발하는 대신 존재하는 소프트웨어를 재사용, 재제작 하기로 마음먹는다. 두가지 프로그램을 눈여겨 보게 되었는데 오승홍씨의 페치팝 과 칼 해리스의 팝클라이언트였다.
POP에 대한 기능이 필요했던 저자는 페치팝에 개선사항을 추가했다. 하지만 그는 한가지 교훈, '갖고 있는 것을 버릴 계획을 세우라. 언젠가는 버리게 될 것이다.'를 떠올리며 페치팝을 계속 발전시키기 보다는 팝클라이언트로 옮겨간다. 페치팝은 오직 pop3만 지원하는 반면 팝클라이언트는 여러 프로토콜을 지원하고 있었던 점이 주요했다. 올바른 방법을 찾기 위해 첫번째 시도(페치팝)을 과감히 버렸다.
칼은 팝클라이언트에 흥미를 잃은 상태였고 저자는 그것을 개선할 아이디어가 있었다. 오픈소스의 문화에서 흔히 그러하듯이, 저자는 그의 프로젝트를 넘겨받았다.

## 사용자가 있다는 것의 중요성
저자가 팝클라이언트 사용자들을 넘겨받았다는 것도 중요하다. 사용자가 있다는 것은 매우 좋은 일이다. 당신이 누군가의 필요를 충족시켜주고 있으며 일을 잘 해 나가고 있다는 것을 보여주기 때문만은 아니다.
적절하게 유도한다면 사용자는 공동 개발자가 될 수도 있다. 조금만 격려해주면 사용자들은 문제를 분석하고 해결책을 제시하며, 도움 없이 혼자 일할 때보다 훨씬 빨리 코드를 개선하도록 해준다.
돌아보면, 리눅스의 성공과 방법론은 GNU 이맥스 리스프 라이브러리와 리스프 코드 아카이브에서 그 선례를 찾아볼 수 있다.
이맥스의 C 코드 핵심이나 대부분의 다른 FSF 도구들의 성당 건축 방식과 대조적으로 리스프 코드 풀의 진화는 유동적이고 사용자가 주도했다.
아이디어와 이맥스 모드들의 원형은 안정적인 최종 형태를 갖추기까지 종종 서너 번씩 다시 쓰였다. 느슨하게 묶인 공동 작업이 인터넷으로 인해 가능해졌고, 리눅스에서처럼 매우 자주 일어나는 일이 됐다.

사실 페치메일 이전에 나 자신의 가장 성공적인 해킹은 아마 이맥스 VC 모드였을 것이다.
세 명의 사람들과 이메일로 리눅스와 비슷한 협동 작업을 했고, 지금까지 그 중 한 명인 (이맥스의 저자면서 자유 소프트웨어 재단의 설립자인) 리처드 스톨먼만을 만나 보았다.
VC 모드는 SCCS, RCS, CVS를 위한 이맥스 안의 프런트엔드였고, ‘원 터치’ 판 관리 기능을 제공했다.09 이것은 누군가 만들어 놓은 작고 조악한 sccs.el 모드로부터 진화한 것이다.
VC의 개발은 이맥스와는 다르게 이맥스 리스프 코드가 발표와 테스트, 개선의 주기를 매우 빨리 반복할 수 있었기 때문에 성공했다.

코드를 법적으로 GPL에 묶어 두려는 FSF의 정책은 한 가지 예기치 못한 부작용을 가져왔다. 그것은 FSF가 시장 개발 방식을 사용하는 절차가 까다로워졌다는 점이다.
이는 저작권법 체계에서 생길 수 있는 문제에 대비해 GPL 코드를 면역시키기 위해 20행 이상의 개인적 공헌에 대해서는 저작권을 양도받아야 한다고 FSF가 믿기 때문이다.
BSD와 MIT의 ‘X 컨소시엄 이용허락 라이센스’을 사용하는 사람에게는 이런 문제가 없다. 그들은 누군가가 문제를 일으킬 동기가 될만한 권리를 가지려 하지 않는다.

## 일찍, 그리고 자주 발표하라
일찍, 자주 릴리즈 하는 것은 리눅스 개발 모델에서 중요한 부분이다. 하지만 초기에 이는 사소한 프로젝트에 적용하는 것이 아니라면 좋지 않은 정책이라 평가 받았다. 왜냐하면 초기 버전에는 버그가 많고 이는 사용자의 인내심을 시험할 수 있었기 때문이었다. 이러한 평가로 인해 성당형 개발 방식이 선호되어왔다. 성당형 개발 방식은 6개월 혹은 그보다 덜 자주 릴리즈 하며 그 동안의 기간에 개처럼 일하는 방식을 추구했다. 하지만, 1년 후 리눅스가 널리 알려지면서 이전보다 훨씬 바람직한 일이 일어나는 것이 분명했다. 리누스의 공개 개발 정책은 성당형 방식과는 완전히 반대였다. 리눅스의 성장은 전례 없는 빈도의 릴리즈 정책에 의해 주도됐다.
“보는 눈이 많으면 모든 버그는 쉽게 찾을 수 있다”
필자는 이를 리누스의 법칙이라고 부른다. 필자의 원래 공식은 “누군가에게는 간단할 것이다” 이었지만, 리누스는 “누군가는 문제를 발견하고, 누군가는 그것을 이해한다. 그리고 나는 문제를 발견하는 것이 더 큰 도전이라 말할 수 있다”라는 이야기를 하였다. 여기에 성당과 시장 스타일의 근본적 차이가 있다. 성당 스타일의 개발에서는 버그와 개발 문제는 까다로우며 이를 해결하기 위해서는 소수의 사람들이 수개월의 조사를 거쳐야 하기 때문에 긴 릴리즈 간격을 가지게 되며, 오랜 기간 기다려온 릴리즈가 완벽하지 않을 때 필연적으로 실망이 따라온다. 하지만, 시장 스타일의 개발에서는 버그는 쉽게 해결되는 문제로 생각한다. 실제로 매번 새로운 릴리즈가 나올 때마다 수천 명의 공동 개발자에게 노출 되며 매우 빠르게 해결 된다. 리누스의 법칙은 수년 전 사회학자들에게도 발견 되었는데, 비슷한 수준의 관찰자들의 평균적인 의견이 이들 중 무작위로 선택된 한 명의 의견보다 훨씬 신뢰 할 만 하다는 것을 확인했으며 이를 ‘델파이 효과’라 불렀다.

## 어떻게 수많은 사람들이 복잡함을 다루는가
시장 방식 개발이 디버깅과 코드의 발전을 크게 가속시켰다.
이를 이해하기 위한 예로, 주로 코드를 모르는 일반 사용자가 제출한 버그 리포트는 표면적인 증상만을 알려줘서 개발자에게 크게 도움이 되지 못하는데 반해 코드를 아는 사람이 제출한 버그 리포트는 개발자가 버그를 수정하는데 크게 도움이 된다.
이를 통해 공유된 소스를 바탕으로 프로젝트를 진행하는 것은 핵심 개발자의 시간을 아낄 수 있다는 점을 알아낼 수 있다.
기존에 널리 통용되던 브룩스의 법칙에 의해 프로젝트의 개발자가 늘어날수록 개발 속도가 지체된다는 편견이 있었지만 오픈소스 프로젝트에서는 브룩스의 법칙이 핵심 개발자 그룹에게만 적용되기 때문에 오픈소스 프로젝트에 참여하는 사람이 늘어도 개발 속도는 지체되지 않는다.
다양한 증상으로 발현되는 복잡한 에러의 경우에는 간단하고 만들어내기 쉬운 버그보다는 찾기가 매우 어렵다. 따라서 버그가 존재하는 곳을 찾을 때 여러 사람이 동시에 다른 코드를 보면서 찾는것이 실력이 뛰어난 소수의 사람이 순서대로 찾는것보다 훨씬 빠르게 찾을 수 있다. 또한 버그를 찾게 되면 다른 사람들도 그 사실을 알게 되어 더이상 버그 찾는 일에 시간을 낭비하지 않을 수 있다.

## 장미가 장미 다우려면
필자는 리누스의 행동을 연구하고 왜 그것이 성공했는 지 생각하며 새 프로젝트에서 이 이론을 시험해보기로 결정했다. 이는 다음과 같은 방법으로 진행하였다.
-일찍 그리고 자주 릴리즈 하기
-페치 메일에 대한 연락을 한 모든 사람을 베타 테스터 목록 에 추가하여 프로젝트를 성장시켰다.
-릴리즈 할 때마다 베타 테스터 목록에 발표를 보내 많은 사람들의 참여를 독려했다.
-베타 테스터들의 의견을 듣고 결정 사항을 투표하며 패치 및 피드백을 보내올 때마다 이들을 구슬렸다.
이 단순한 방법들은 즉각적인 효력을 보였으며, 훌륭한 비판, 버그리포트, 수정 코드를 받을 수 있었다. 이 시험을 통해 ‘베타 테스터를 가장 중요한 자원으로 여긴다면 그들은 가장 귀중한 자원이 될 것이다’ 라는 결론을 이끌어 낼 수 있었다.

## 팝클라이언트가 페치메일이 되다.
페치메일 프로젝트에서 큰 전환이 일어났던 것은 Harry Hochgeiser가 클라이언트 컴퓨터의 SMTP 포트로 메일을 포워딩하는
대략적인 코드를 보내준 때였다. 이 기능을 구현한다면 다른 딜리버리 방법은 구식이 된다는 것을 깨달았다.
여러 주 동안 페치메일을 조금씩 뜯어고쳤는데, 인터페이스 설계가 작동하긴 했지만 지저분하다고 느끼고 있었다. 우아하지도 않고 몇 안 되는 옵션들이 너무 여기저기 흩어져 있었다.
가져온 메일을 메일상자 파일에 부어놓을 것인지, 표준 출력으로 내보낼 것인지 결정하는 옵션이 특히 골칫거리였지만 왜 그런지 확실히 깨닫지는 못했다.
SMTP 포워딩을 생각하자 그동안 팝클라이언트가 너무 많은 것을 해내려고 했다는 것을 알게 됐다. 팝클라이언트는 MTA와 MDA의 기능을 모두 갖추도록 설계됐다.
SMTP 포워딩만 할 수 있다면 MDA 기능을 없애고 순수한 MTA가 될 수 있었다. 센드메일과 마찬가지로 최종적인 메일 배달은 다른 프로그램에 맡기면 된다.
몇 가지 배울 점이 있다면 SMTP 포워딩에 대한 아이디어는 리누스의 방법을 모방하려고 의식적으로 노력한 것에 대한 가장 큰 보답이었다.
사용자 한 명이 정말 좋은 아이디어를 주었으며, 저자는 그 의미를 이해만 하면 되었다.
팝클라이언트를 MTA와 MDA 기능을 다 갖추고 복잡한 지역 딜리버리 모드까지 갖춘 것으로 개발해 나가면서 잘못된 문제를 풀려고 노력하고 있다.
페치메일의 설계는 가장 기초적인 것부터 재고해서 SMTP 포트로 메일을 딜리버리하는 인터넷 메일 경로의 핫 부분인 MTA가 되어야 했다.

만약에 개발 도중에 어려움을 겪는다면, 그 때에는 정답을 가졌는지가 아니라 질문이 올바른 것인지 의문을 가져봐야 하는 경우가 있다. 이 때는 문제의 틀을 다시 잡아야 할 것이다.
저자는 문제의 틀을 다시 잡았다. 1. SMTP 포워딩 지원 기능을 일반 드라이버에 포함한다. 2. SMTP 포워딩을 기본 모드로 만든다. 3.마지막으로 다른 딜리버리 모드를 특히, '파일 딜리버리'
과 '표준 출력으로 딜리버리'를 제거해야 했다.
3단계 에서 힘들었는데, 그 이유는 팝클라이언트를 사용하면서 다른 딜리버리 모드에 의존하는 사용자의 마음을 불편하게 만들고 싶지 않아서였다.
포워드 파일이나 센드메일 외의 비슷한 프로그램으로 전환하여 동일한 결과를 얻을 수 있었지만, 실제로는 다른 프로그램으로 전환하는 것 자체가 큰일이 된다.
우려했던 것과 달리 3단계를 실행하고 이점이 매우 많은 것으로 나타났다. 드라이버 코드 중 가장 힘든 부분이 사라졌고 시스템의 MDA와 사용자의 메일 상자를
굳이 다 찾아다닐 필요가 없어졌고, OS가 파일 잠금을 지원하는지 걱정할 필요도 없어졌다.
또한 성능도 향상됐다. 변경에 따른 그다지 중요하지 않은 또 하나의 이점이라면 메뉴얼 페이지가 훨씬 간단 해졌다는 것이다.
나중에 저자는 사용자가 지정한 지역 MDA를 통해 배달하는 기능을 다시 넣어야 했다. 동적 SLIP을 포함해 몇몇 애매한 상황을 다뤄야 했기 때문이다. 하지만 처음보다 훨씬 간단한 방법을 찾아낼 수 있었다.
코드가 더 나아지고 간단해지고 있을 때가 바로 일이 제대로 되어가고 있다는 것을 알게되는 때이다. 그 과정에서 페치메일의 설계는 조상 격인 팝클라이언트와 다른 자신만의 정체성을 갖게 된다.
이름을 바꿀 때가 된 것이다. 새로운 설계는 예전의 팝클라이언트보다 센드메일과 비슷해 보였다. 둘다 MTA였지만 센드메일은 PUSH후에 메일을 딜리버리했고 새로운 팝클라이언트는
PULL후에 메일을 딜리버리했다. 그래서 두 달후에 저자는 팝클라이언트의 이름을 페치메일로 변경했다.

## 페치메일의 성장
페치메일은 이제 다양한 프로토콜의 지원으로 '카테고리 킬러'가 될 경쟁력을 갖춘 프로그램이 되었다. 하지만 이것은 처음부터 저자가 '위대한 도구'를 만드려는 목적을 가지거나 '독창적인 아이디어'에서 온 것이 아니었다. 다른 사람의 아이디어를 가지고 와서 더 멀리 끌고 가 구체화해서 성공한 리눅스처럼, 그 또한 칼과 해리의 아이디어를 가져와 밀어붙인 결과, 페치메일을 만들어낼 수 있었다.
그는 곧 자신과는 상관 없지만 다른사람에게는 필수적인 기능을 포함하고 지원해야 함을 깨달았고 '멀티드롭'과 '8비트 MIME' 작업에 착수한다. 멀티드롭 기능의 추가는 저자의 기대 뿐만 아니라 메일링 리스트를 운영하는데도 사용되면서 전혀 기대하지 않았던 용도에 알맞게 될 수도 있음을 깨닫는다.
또한 수신자가 강제하지 않는다면 정보를 절대로 잘라버리지 말라는 규칙을 따라 프로그램을 개발한 결과 8비트 MIME 작업은 버그없이 간단히 해낼 수 있었다.

## 페치메일에서 배울 점
일반적인 소프트웨어 공학 주제로 돌아가기 전에 페치메일의 경험에서 배울 점이 몇 가지 더 있다.
RC파일 구문은 선택 사항으로 '노이즈'라는 키워드를 포함한다. RC파일에서 허용하는 영어와 비슷한 구문은 잘라낼 것을 모두 잘라내고 얻은 전통적이고 간명한 키워드와 값의 쌍에 비해 훨씬 알아보기 쉽다.
이것은 저자가 RC파일의 선언들이 소언어를 얼마나 많이 닮아가기 시작했는지 알아차린 뒤 실험에서 시작됐다.('서버'라는 키워드를 '폴'로 바꾼 이유도 이것이다.)
전통적인 프로그래머들은 정확하고 짧으며 중복을 허용하지 않는 제어 구문을 선호하는 경향이 있다. 컴퓨팅 자원이 비싸서 구문 분석 단계가 최대한 싸고 간단해야 했을 때부터 내려온 문화적 유산이다.
저자가 영아와 비슷한 구문을 일반적으로 피하는 이유는 아니다. 언급한 이유는 그런 관습을 없애기 위해서이다. 예를 들어 CPU와 메모리 가격이 싸졌는데도 간명한은 저절로 없어지지 않았다.
물론 조심해야할 충분한 이유가 있다. 한 가지는 구문 분석 단계의 복잡성에 대한 비용이다. 구문 분석 단계를 버그가 우글거리면서 사용자로 하여금 그 자체만으로 혼란을 느끼게 만들고 싶지는 않을 것이다
또 하나의 이유는 언어의 구문을 영어와 비슷하게 만들려고 노력하면 그 ‘영어’가 심각하게 왜곡돼 자연어와의 피상적인 유사점이 전통적인 구문만큼이나 혼란스럽게 되는 경우가 많다는 점이다.
언어의 영역이 매우 제한돼 있기 때문에 페치메일 제어 구문에서는 이런 문제를 피하려고 했다. 일반적인 목적의 언어와는 거리가 멀었다.
언어가 표현하는 것이 별로 복잡하지 않았기 때문에 영어의 아주 작은 하위 집합에서 실제 제어 언어로 옮겨가는데 혼란을 일으킬 가능성이 적었다. 더 넓은 의미의 교훈을 여기에서 얻었다.
또 하나의 교훈은 불투명함에 의한 보안이다. 페치메일 사용자 중에는 스누퍼snooper가 우연히 비밀번호를 보지 못하도록 rc 파일에 있는 비밀번호를 암호화하자고 말하는 사람이 있었다.
저자는 그 말을 받아들이지 않았는데, 그렇게 한다고 해서 보안이 강화되는 것이 아니기 때문이다.
rc 파일의 읽기 권한을 얻은 사람이라면 사용자와 마찬가지로 페치 메일을 실행시킬 수도 있다. 그리고 그들이 비밀번호를 원한다면 비밀번호를 얻기 위해 페치메일 코드에서 디코딩하는 코드를 뽑아낼 수도 있다.
'보안 시스템은 그것이 보호하려는 비밀만큼만 안전하다. 가짜 비밀에 주의하라'

## 시장 방식 개발에 필요한 선행조건들
처음부터 프로젝트를 시장 방식으로 개발하는것은 매우 어렵다. 그래서 다른 개발자들을 끌어들이기 위해서는 그들을 위한 장난감, 다시 말해 개발자들을 끌어들일만한 유인이 있어야 한다.
그 유인중에 하나는 프로젝트의 장래성이다. 개발자 공동체를 만들기 시작할 때 머지 않은 미래에 이 프로젝트가 정말 괜찮은 무언가가 될 수 있다는 생각을 다른 개발자들이 하도록 만들어야 한다.
또 다른 유인중에 하나는 의사소통 기술이다. 개발자도 결국 사람이기 때문에 그들에게 흥미를 주어야 하고 그들이 내놓은 결과에 대해 기분 좋게 만들어주어야 프로젝트에 매력이 생길 것이다.

## 오픈소스 소프트웨어의 사회적 문맥
"재미있는 문제를 풀어보고 싶다면, 자신에게 재미있는 문제를 찾아 나서는 것부터 시작하라."
기존 소프트웨어 이론은 지연되는 프로젝트에 개발자를 더 투입하는 것은 완료 시기를 더 늦출 뿐이라 말했다.
복잡성과 의사소통에 드는 비용이 개발자 수의 제곱에 비례하는 반면 작업 결과는 선형으로만 증가한다고 주장했었으나, 브룩스의 법칙이 전부였다면 리눅스는 불가능했을 것이다.
자아를 내세우지 않는 프로그래밍이란 개발자들이 자신의 코드에 텃세를 부리지 않고 다른 사람으로 하여금 버그를 찾고 개선가능성을 찾아내도록 격려하는 곳에서 다른 어느 곳에서보다 극적으로 빠른 개선이 일어나는 프로그래밍이다.
전통적인 유닉스 세계에서 자아를 내세우지 않는 프로그래밍을 내세울수 없는 요인은 첫째, 다양한 이용허락의 법적인 제약, 영업비밀, 상업적인 이해관계에 의해, 둘째, 인터넷이 훌륭하지 못했기 때문 -> 지리적으로 좁은 지역에 공동체가 자리잡고 있었기 때문이다.
리눅스와 월드 와이드 웹의 탄생이 일치하던 것은 결코 우연이 아니다. 리눅스는 급속히 보급된 인터넷을 가능하게 했던 그 규칙에 따라 어떻게 일을 진행해야 하는지 알았던 최초의 사람이고, 그는 인터넷의 발전과 리더십 방식과 협력하는 관습의 발전에 의해 매체를 최대한 사용하게 햇다.
리눅스 프로젝트는 많은 사람의 의지를 수렴해 노력하는 것을 요구한다. 브룩스 법칙에 반해, 개발 조정자가 최소한 인터넷만큼 좋은 매체를 갖고 있으며 강제력을 사용하지 않고 어떻게 이끌어야 할 지 알고 있다면, 한 명 보다는 여러 명의 지도자가 필연적으로 낫다.
개인의 비전과 똑똑함보다는 오픈소스 소프트웨어의 최첨단은 개인의 비전과 똑똑함에서 시작해 자발적으로 흥미를 보이는 공동체를 효과적으로 구축해서 그것을 증폭시키는 사람들에게 속할 것이다.
최종적으로 협동이 더 도덕적이라거나 소프트웨어 매점이 덜 도덕적이라서가 아니라 단지 폐쇄 소스 측과 오픈소스 공동체와의 군비 경쟁에서 오픈소스 측이 한 문제에 훨씬 큰 비율로 숙련된 사람의 시간을 쏟을 수 있기 때문에 오픈소스 문화가 승리를 거둘 것이다.
