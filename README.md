# 🌄 기상청 : 지면온도 예측
![69744314](https://github.com/user-attachments/assets/c19b2e84-a357-4ddf-be78-2e8fbd40e1f0)
![76687996](https://github.com/user-attachments/assets/fa51738c-7890-45c2-b8d3-05715d756093)
![94885063](https://github.com/user-attachments/assets/dcc28d77-814b-44bf-b0a7-daaede6211f6)
![105350096](https://github.com/user-attachments/assets/2fad07e0-8441-46fd-8f4b-60870260e3f9)

## Abstract
> 지면온도 예측 모델을 만들고 이에 관해 설명 및 해석을 진행한다.

<h2> 👪 Team </h2>

> Name : AutoWeather is real

<h3> 👪 Members </h3>
<table>
  <tr>
    <td> <div align=center>  1 </div> </td>
    <td> <div align=center>  2 </div> </td>
    <td> <div align=center>  3 </div> </td>
    <td> <div align=center>  4 </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b>김다운</b> </div> </td>
    <td> <div align=center> <b>오지우</b> </div> </td>
    <td> <div align=center> <b>오지우</b> </div> </td>
    <td> <div align=center> <b>오지우</b> </div> </td>
  </tr>
  <tr>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/c19b2e84-a357-4ddf-be78-2e8fbd40e1f0" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/fa51738c-7890-45c2-b8d3-05715d756093" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/dcc28d77-814b-44bf-b0a7-daaede6211f6" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/2fad07e0-8441-46fd-8f4b-60870260e3f9" width="200" height="300"/> </td>
  </tr>
  <tr>
    <td> <div align=center> <a href="https://github.com/Daw-ny"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/woooyen"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/woooyen"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/woooyen"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
  </tr>
</table>

<h3> 🛑 Role & Rule </h3>

> ### Ground Rule
> - 각자 데이터를 활용할 방법에 대해 생각해보고 생각대로 진행한다.
> - 회의를 통해 각자의 역할을 정하고 다음 회의까지 진행된 상황을 공유하여 서로의 피드백을 듣고 필요한 부분은 수정한다.
> - 휴식시에는 꼭 다같이 쉴것.


<table>
  <tr>
    <td> <div align=center> <b> 이름 </b> </div> </td>
    <td> <div align=center> <b> 역할 </b> </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 김다운 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br> 
	 <b>모델링 진행 </b>(봄, 여름 맞춤형 모델 생성)</br>
	 <b>파생변수 생성 </b>(기상정보에서 나타날 수 있는 변수들을 생성)</br>
	 <b>코드 및 데이터 정리 </b>(활용한 코드 및 데이터 정리 및 취합) </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 오지우 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br>
	 <b>모델링 진행 </b>(가을, 겨울 맞춤형 모델 생성)</br>
	 <b>반응 변수 변환 </b>(log 또는 boxcox변환을 통한 관계 변화 적용)</br>
	 <b>코드 및 데이터 정리 </b>(활용한 코드 및 데이터 정리 및 취합) </td>
  </tr>
</table>

<h3> 📽️ Project Intro </h3>

<table>
  <tr>
    <td> <div align=center> <b> Subject </b> </div> </td>
    <td> 계절별로 달라지는 지면온도에 대해 예측할 수 있는 모델을 만들고 그에따른 의미를 해석 </td>
  </tr>
  <tr>
    <td> <div align=center> <b> Processing </b> </div> </td>
    <td> 1. 데이터의 각 칼럼이 어떤 의미를 갖는지 확인하고 각 칼럼의 분포 및 결측, 이상치 존재여부 확인 </br>
  	 2. 이상치 및 결측치를 대치 처리하고 파생변수를 생성하여 맞춤 성능을 파악하면서 피팅 조절 </td>
  </tr>
  <tr>
    <td> <div align=center> <b> Develop Enviroment </b> </div> </td>
    <td> <tt>Tool</tt>: Jupyter Notebook</td>
  </tr>
  <tr>
    <td> <div align=center> <b> Communication Enviroment </b> </div> </td>
    <td> <tt>Notion</tt>: 프로젝트를 위한 역할분담, 아이디어 브레인 스토밍, 프로젝트 관련 회의 내용 기록 </br>
	 <tt>Zoom, Offline Meeting</tt>: 실시간 대면/비대면 회의 </td>
  </tr>
</table>

<h3> 📆 Project Procedure </h3>

>  자세한 진행 내용은 [notion](https://www.notion.so/d52a18bf33b5403896132cc05fdbedaa?pvs=4)에서 확인하실 수 있습니다.

<h3> 📂 Project Structure </h3>

> - Code
>> 각 방법을 이름에 따른 방법으로 적용하면서 반복 실행하였습니다. 파일을 주로 모델링 방법에 따라서 나누었습니다.

<h3> ⚙️ Architecture </h3>
<table>
  <tr>
    <td> <div align=center> <b> 분류 </b> </div> </td>
    <td> <div align=center> <b> 내용 </b> </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 모델 </b> </div> </td>
    <td> <tt>MLjar-supervised(AutoML)</tt> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 데이터 </b> </div> </td>
    <td> 제공해준 기상청 데이터 자료 (외부 데이터 사용 금지), 일출 및 일몰 시각(참조용) </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 모델 평가 및 해석 </b> </div> </td>
    <td> SMAPE를 계산하여 모델의 개선점 확인, 계절별로 산출 후 평균을 내어 최종 스코어 선정 </td>
  </tr>
</table>
