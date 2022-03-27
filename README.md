# 분산 Edge Cloud 환경에서 <br/>Event 기반 Function-as-a-Service 기능 개발<br/>[![license](https://img.shields.io/github/license/dohyunKim12/FaaS-Soong.svg?style=flat-square)](https://github.com/dohyunKim12/FaaS-Soong/blob/master/LICENSE)

> :trophy: 2021년 **NET CHALLENGE CAMP SEASON8 GOLD AWARD**. 숭실대학교 팀 빠숭(FaaSoong)<br/>
https://www.youtube.com/watch?v=UieUycoFO5o

## Summary
KEDA(Kubernetes-Event-Driven-AutoScaling)을 활용한 Scale-to-Zero 구현. 

평상시에 동작하지 않는 상태에서 이벤트 발생 기반으로 서비스 생성 및 Scale-Out 하는 Serverless Computing Model을 구현한다. Edge-Cloud 환경에서 Event 기반으로 동작하는 응용 예로서 특정 상황 발생 시(예: 교통사고 발생 등) CCTV가 복잡한 인식기능을 하는 외부 OpenService를 이용하여 해당 사건을 처리하는 여러 서비스를 필요한 곳에 제공하는 FaaS(Function as a Service) Model을 구현한다.

## Developers
**숭실대학교 전자정보공학부**

* [김도현](https://github.com/dohyunKim12)(Dohyun Kim)
* [송수현](https://github.com/suhyunS123 )(Suhyun Song)
* 송지원(Jiwon Song)
* [윤창섭](https://github.com/ryunchang)(Changseop Yoon)

## Scope
**Point of Infrasturcture**  
- Kubernetes를 활용한 Cluster 구축.
- Cluster Monitoring을 위해 Prometheus와 Grafana를 설치.
- KEDA 및 RabbitMQ Server 설치.

**Point of Service**  
- 사고 상황을 감지하는 Deep Learning Model을 FaaS로써 배포.  
- 상황 감지를 단계적으로 구현함으로써 자원 효율성을 극대화.
- OpenCV를 이용하여 움직임을 감지하는 애플리케이션을 워커 노드에서 동작.
- 이벤트 기반의 함수형 서비스 제공.

## Overall Architecture

<img src="https://user-images.githubusercontent.com/72643027/153318004-74439fbb-4aa9-4086-90e9-e3f43589fe71.png" width="70%" height="70%"/>

## Scenario

![64mssl](https://user-images.githubusercontent.com/72643027/153319790-42679e44-bd3e-4524-a3d0-b22bac2c68f5.gif)

## GPU Resource Monitoring

![64mrtb](https://user-images.githubusercontent.com/72643027/153318969-e2c350e7-ca8b-42da-9c5f-309eab4e6720.gif)

<br/>

**For more, please check out `doc/`**
