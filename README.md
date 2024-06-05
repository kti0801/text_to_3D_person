# text_to_3D_person

### <p>$\bf{\large{\color{#1589F0}주제}}$ 감성분석과 3D를 활용한 캐릭터 생성 </p>
#### <p>$\bf{\large{\color{#1589F0}기획}}$ GAN 모델을 사용해 다양한 표정의 이미지를 생성하고, 이를 3D 모델링으로 변환하여 동화책의 텍스트 감성 분석에 따라 맞춤형 감정 표현을 제공하는 시스템을 개발 </p>

> 파이널 프로젝트 - [비정형 데이터] 객체인식 모델을 활용한 안면분류 모델 구현
>> (2자 목표) 안면 분류 모델을 활용한 서비스 제공 프로젝트

#### 프로젝트 기간: (2024) 5월 9일(목) ~ 6월 5일(수) (약 4주)
#### 팀원: 김토일, 심재은, 이상윤, 허영민

* 데이터 (출처) ESTSOFT 제공
  * Train Data : 약 6000장
  * Validation Data: 약 1200장
  * Test Data: 약 1200장

![분류](https://github.com/LeeSY99/text_to_3D_person/assets/74341916/9c5c23c0-7a53-49d0-9591-c4e1256faad8)
<br/>
<br/>

<div align=left><h1>📚 STACKS</h1></div>

<div align=left>
 <body>
  Environment
  <p>
   <img src="https://img.shields.io/badge/Google Colab-F9AB00?style=for-the-badge&logo=Google Colab&logoColor=white"> 
   <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">
  </p>
 </body>
  <br>
 
<div align=left>
 <body>
  Development
  <p>
   <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> 
   <img src="https://img.shields.io/badge/Tensorflow-FF6F00?style=for-the-badge&logo=Tensorflow&logoColor=white">
   <img src="https://img.shields.io/badge/Pytorch-EE4C2C?style=for-the-badge&logo=Pytorch&logoColor=white"> 
   <img src="https://img.shields.io/badge/Blender-E87D0D?style=for-the-badge&logo=Blender&logoColor=white"> 
  </p>
 </body>
  <br>
 
<div align=left>
 <body>
  Communication
  <p>
  <img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=Discord&logoColor=white">
  <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white">
  </p>
 </body>
  <br>
 
## 주요 모델 기술
* DECA
  #### &rightarrow; 얼굴표정, 주름, 세부사항을 추출할 수 있어 표정 표현에 좋기에 모델 선정
<br/>
※ 참고문헌 https://chickenrush.tistory.com/16
<br/>
<br/>

## Data Augmentation
* face-detection: [ibug.face_detection](https://github.com/hhj1897/face_detection)
* face-alignment: [ibug.face_alignment](https://github.com/hhj1897/face_alignment)
* face-augmentation: [ibug.face_pose_augmentation](https://github.com/hhj1897/face_pose_augmentation)

![Aug_example](https://github.com/LeeSY99/text_to_3D_person/assets/101381138/b7621711-f780-46ef-87b1-33ed8d7ad176)


## 3D Model Avatar
* StarGAN
* 3DMM
* DECA

![Input_stage](https://github.com/LeeSY99/text_to_3D_person/assets/101381138/0ac81b2f-67f8-4879-bdc2-eef50a3fac01)
![StarGAN&DECA](https://github.com/LeeSY99/text_to_3D_person/assets/101381138/07d70693-abd5-4dd6-970f-3579f783525f)
![3D model avatar](https://github.com/LeeSY99/text_to_3D_person/assets/74341916/105176de-3fd5-43fa-9387-e5cf128c6a08)

* Text Classfication (KoElectra)


## 구현 영상

<video controls src='https://github.com/LeeSY99/text_to_3D_person/assets/101381138/b265ee8c-3347-4751-a19b-a4416c6fc6b0'></video>

## 개선 및 보완 방향
* 더 다양한 감정 표현을 위해 GAN 모델을 개선하고, 실시간으로 감정을 분석하고 반영하는 기능을 추가할 계획
* 더 자연스러운 3D모델 발전.