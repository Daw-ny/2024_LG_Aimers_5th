# 🌄 기상청 : 지면온도 예측

## Abstract
> 최근 기계학습 모델의 발전과 함께 제품의 생산 단계에서 이상 여부를 미리 판단하려는 시도가 증가하고 있습니다. 이번 경진대회에서는 공정 과정의 여러 가지 데이터를 이용해 이상 여부를 판별하는 모델을 구현하고 그 성능을 비교하고자 합니다.

<h2> 👪 Team </h2>

> Name : 쿼드비트

<h3> 👪 Members </h3>
<table>
  <tr>
    <td> <div align=center>  1 </div> </td>
    <td> <div align=center>  2 </div> </td>
    <td> <div align=center>  3 </div> </td>
    <td> <div align=center>  4 </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b>손동현</b> </div> </td>
    <td> <div align=center> <b>김다운</b> </div> </td>
    <td> <div align=center> <b>서상혁</b> </div> </td>
    <td> <div align=center> <b>서준혁</b> </div> </td>
  </tr>
  <tr>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/c19b2e84-a357-4ddf-be78-2e8fbd40e1f0" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/fa51738c-7890-45c2-b8d3-05715d756093" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/dcc28d77-814b-44bf-b0a7-daaede6211f6" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="https://github.com/user-attachments/assets/2fad07e0-8441-46fd-8f4b-60870260e3f9" width="200" height="300"/> </td>
  </tr>
  <tr>
    <td> <div align=center> <a href="https://github.com/stat-thon"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/Daw-ny"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/devhyuk96"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/SeoBuAs"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
  </tr>
</table>

<h3> 🛑 Role & Rule </h3>

> ### Ground Rule
> - 실시간 접속을 기본으로 진행하되 일정이 있는 인원은 각 일정을 마치고 접속
> - 일주일에 한번 정기회의를 진행하며 그동안 진행했던 경과 및 실험 결과를 공유하고 앞으로 어떤 전략을 취할지 토론
> - 새로운 정보가 생겨날 때 실시간 전달


<table>
  <tr>
    <td> <div align=center> <b> 이름 </b> </div> </td>
    <td> <div align=center> <b> 역할 </b> </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 손동현 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br> 
	 <b>모델링 진행 </b>(과정 단계별 분할 및 결과 앙상블)</br>
	 <b>데이터 형질 변환 </b>(연속형 변수 범주화, 선택형 범주화 적용)</td>
  </tr>
  <tr>
    <td> <div align=center> <b> 김다운 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br>
	 <b>모델링 진행 </b>(Stratified 10-CV 적용, stage 단계별 모델링 및 앙상블 적용)</br>
	 <b>데이터 조정 </b>(밀림 데이터 처리 및 잘못 기입된 값 평행이동 보정)</td>
  </tr>
  <tr>
    <td> <div align=center> <b> 서상혁 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br>
	 <b>모델링 진행 </b>(Stage별 적합 및 앙상블, 최대 과정 10개의 대형 앙상블 적용, 기초 모델 코드 작성)</br>
	 <b>파생변수 생성 </b>(각 공정 과정에서 발생할 수 있는 파생변수 생성) </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 서준혁 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br>
	 <b>최적 모델 탐색 </b>(임계값 조정을 이용한 데이터 불균형 해소, 파라미터 세부 조절)</br>
	 <b>데이터 조정 </b>(밀림 데이터 처리 및 잘못 기입된 값 평행이동 보정)</td>
  </tr>
</table>

<h3> 📽️ Project Intro </h3>

<table>
  <tr>
    <td> <div align=center> <b> Subject </b> </div> </td>
    <td> 디스플레이 2가지를 합성하는데 발생할 수 있는 불량 탐지 </td>
  </tr>
  <tr>
    <td> <div align=center> <b> Processing </b> </div> </td>
    <td> 1. 데이터의 각 칼럼별 의미 해석 및 잘못 기입과 같은 실수로 인한 이상치 처리 </br>
  	 2. 파생변수 및 최적 모델을 위한 파라미터 탐색으로 출력한 F1-score을 비교해 가장 높은 값을 갖는 모델 선정 </td>
  </tr>
  <tr>
    <td> <div align=center> <b> Develop Enviroment </b> </div> </td>
    <td> <tt>Tool</tt>: Jupyter Notebook</td>
  </tr>
  <tr>
    <td> <div align=center> <b> Communication Enviroment </b> </div> </td>
    <td> <tt>Notion</tt>: 과정 혼동을 방지하기 위한 기록, 아이디어 브레인 스토밍, 프로젝트 관련 회의 내용 기록 </br>
	 <tt>Zoom, Offline Meeting</tt>: 실시간 대면/비대면 회의 </td>
  </tr>
</table>

<h3> 📆 Project Procedure </h3>

>  자세한 진행 내용은 [notion](https://sixth-drum-9ac.notion.site/LG-Aimers-5-7f95cb60d0164a279ae2e6575f7b8e80?pvs=4)에서 확인하실 수 있습니다.

<h3> 📂 Project Structure </h3>

> - Code
>> 각 방법을 이름에 따른 방법으로 적용하면서 반복 실행하였습니다. 파일을 주로 모델링 방법에 따라서 나누었습니다.  
>> Direction 1: 주로 결측치 또는 이상치를 처리하거나 데이터의 오류를 보정하는 코드입니다.  
>> Direction 2: 데이터에 대한 내용을 그래프로 표현하거나 데이터 특성을 반영한 파생변수를 만든 코드입니다.  
>> Direction 3: Direction 2에서 큰 의미가 있는 변수를 모아 파생변수로 만든 전처리 코드입니다.  
>> Direction 4: 모델링을 적합한 코드입니다. 파라미터 추정에 Optuna를 주로 사용하였습니다.

<h3> ⚙️ Architecture </h3>
<table>
  <tr>
    <td> <div align=center> <b> 분류 </b> </div> </td>
    <td> <div align=center> <b> 내용 </b> </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 모델 </b> </div> </td>
    <td> <tt>LightGBM</tt>, <tt>XGBoost</tt>, <tt>Catboost</tt> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 데이터 </b> </div> </td>
    <td> Elice에서 제공해준 Sub Assembly 공정 데이터 </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 모델 평가 및 해석 </b> </div> </td>
    <td> 주요 지표인 F1을 통해 최적의 파라미터를 탐색, 세 가지 모델의 추정 확률을 계산하여 최적의 앙상블 비율을 반영, 불균형이 가장 해소되는 임계값을 찾아 불량 판단 확률 임계값을 조정 </td>
  </tr>
</table>
