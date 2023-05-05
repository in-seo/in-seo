<details>
 <summary>
         &nbsp;<a href = "https://soup.pw">스프</a> : 흩어져 있는 스터디와 프로젝트가 모여있는 곳🔹기획, 서버 전체 담당.  <sub>(방문자 1.5만+ , 조회수 17만+, 구글검색 1.1위) (2022.07 ~ 운영중)</sub>
 </summary>
&nbsp;
 
![soup2](https://user-images.githubusercontent.com/94730032/208659106-16f7d859-40e2-4217-832f-5cc04d10e1ff.png)

![20230121_120351](https://user-images.githubusercontent.com/94730032/213840975-14a69d7f-d635-4912-9edc-6623c3e0583b.png)

</details>


 <details> &nbsp;
     <summary>
          &nbsp;<a href = "https://chaksong.com">착송 </a>: 착오송금 반환 서비스 스타트업🔹서버 전체, 은행 API 담당  <sub>(2022.12 - 03.31) 점검중  </sub> 
     </summary>
&nbsp;
 <sub> 
  
  [ 금융기관 선정 서비스 '착송' ] <br>
  
  2022 예비창업패키지(정부지원사업) 선정 서비스 <br>
  
  2022 부산은행 썸인큐베이터 7기 선정 서비스 <br>
  
  2022 부산 창업 촉진 사업 액셀러레이팅 선정 기업 <br>
  
  2022 부산 클라우드 엑스포 전시 서비스 <br>
  
  2022 부산 혁신 창업기업 육성 플랫폼(BIGS) 사업 우수 기업 선정 <br>
  
  <a href = "https://n.news.naver.com/article/014/0004938410">출시 기사 링크</a>
  
 </sub> 
 
![회사소개 삽입 이미지 2 (1)](https://user-images.githubusercontent.com/94730032/201576242-11cdfd72-fe51-46df-909d-4e478c0f91f1.svg)

![(figma) 엑스포 벽면 그래픽 디자인_3 (1)](https://user-images.githubusercontent.com/94730032/201576237-71d333ae-26c9-43c3-8f73-c2fc3968b356.svg)


 </details>
 
<li> <a href = "https://github.com/HIUMC"> UMC 홍익대지부</a> Founder.  서버 파트장🔹스프링 스터디, 프로젝트 리드  <sub>(2022.09 ~ 2023.5)  </sub> </li>
&nbsp;

 <details> &nbsp;
 <summary>
  &nbsp;<a href = "https://sinzak.net">신작 </a>: 신세대의 작품을 만나다. <sub>[Web, IOS, AOS]</sub>🔹기획, 서버, 배포 담당 <sub>(2022.10 ~ 2023.4) 앱 검수중</sub> 
 </summary>
 
  ![sinzak](https://user-images.githubusercontent.com/94730032/201578971-0ddbf27c-4ae5-4f66-bf21-00bdf3c1811b.jpg)
 
 </details>
 
 <details> &nbsp;
 <summary>
         &nbsp;<a href = "https://univcert.com">UNIVCERT </a>: 단 한 줄의 코드로 메일 및 대학 인증 끝내기🔹기획, 디자인, 서버 전체 담당 <sub>(2023.2 ~ 운영중)  </sub> 
 </summary>
 
 ## 🐣 초보자를 위한 UnivCert의 라이브러리 배포

자세한 설명은 [해당 사이트](https://univcert.com/)에서도 확인하실 수 있습니다.

💡 build.gradle에 해당 코드 두 줄 추가

```
repositories{
  ...
  maven {url 'https://jitpack.io'}
}

dependencies{
  ...
  implementation 'com.github.in-seo:univcert:master-SNAPSHOT'
  ...
}
```

✉ 이용자 메일 인증 시작 (인증코드 발송)

**`UnivCert.certify("key", "email", "univName", univ_check(bool));`**

- -> 하단 json 형태로 자동 변환 및 http 전송 POST([univcert.com/api/v1/certify](http://univcert.com/api/v1/certify))

```
{
  “key” : “부여받은 API KEY”,
  "email” : “abc@mail.hongik.ac.kr”,
  “univName” : “홍익대학교”,
  “univ_check” : true
	(true라면 해당 대학 재학 여부, false라면 메일 소유자 인증만)
}
```

✅ 이용자 메일에 발송된 코드를 전달 받아 인증 받기

**`UnivCert.certifyCode("key", "email", "univName", 인증코드(int));`**

- -> 하단 형태로 자동 변환 및 http 전송 POST([univcert.com/api/v1/certifycode](http://univcert.com/api/v1/certifycode))

```
{
  “key” : “부여받은 API KEY”
  “email” : "abc@mail.hongik.ac.kr”,
  “univName” : “홍익대학교”,
  “code” : 3816
}
```

🆗 응답 성공 시 인증 끝 !
 
 </details>
  
