# 푸잉 푸잉

## 프로젝트 계획이유

일반인들은 외국 제품들의 성분표를 쉽게 알지 못하는 경우가 많습니다. 또한, 성분표가 한국어로 표기되어 있더라도 생소한 이름이 많아 어떤 효과나 부작용이 있는지 알기 어렵습니다. 그래서 일반인들이 식품성분표의 사진을 찍으면 해당 사진에 있는 성분들의 이름과 내용을 제공하는 앱을 계획했습니다.

## 알고리즘

![알고리즘](./img/algorithm.png)

앱을 실행한 후 사용자가 성분표를 촬영하거나 갤러리에 있는 사진을 선택하면 OCR을 이용하여 사진에 있는 모든 텍스트를 추출합니다. 추출한 텍스트들을 네이버 번역 API를 이용하여 외국어를 한국어로 번역을 한 후 개체명 인식 API를 이용하여 필요한 정보의 태그(MT_CHEMICAL, TMM_DRUG, FD_MEDICINE, CV_FOOD, CV_DRINK, MT_ELEMENT, MT_METAL)가 있는 단어들을 판별하여 해당 단어들을 추출합니다. 해당 단어들은 위키백과 QA API를 이용하여 성분 및 재료에 대한 위키백과에서 정의하고 있는 자세한 정보들을 출력하여 사용자에게 제공합니다.

## 시퀀스 다이어그램

![시퀀스 다이어그램](./img/se.png)


### 테스트는 이런 식으로 작성하시면 됩니다

```
예시
```

## Deployment / 배포

Add additional notes about how to deploy this on a live system / 라이브 시스템을 배포하는 방법

## Built With / 누구랑 만들었나요?

* [이름](링크) - 무엇 무엇을 했어요
* [Name](Link) - Create README.md

## Contributiong / 기여

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us. / [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) 를 읽고 이에 맞추어 pull request 를 해주세요.

## License / 라이센스

This project is licensed under the MIT License - see the [LICENSE.md](https://gist.github.com/PurpleBooth/LICENSE.md) file for details / 이 프로젝트는 MIT 라이센스로 라이센스가 부여되어 있습니다. 자세한 내용은 LICENSE.md 파일을 참고하세요.

## Acknowledgments / 감사의 말

* Hat tip to anyone whose code was used / 코드를 사용한 모든 사용자들에게 팁
* Inspiration / 영감
* etc / 기타
