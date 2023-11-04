# Kotlin_Null
null 관련 개발 경험 정리
![image](https://github.com/chihyunwon/Kotlin_Null/assets/58906858/47f880a7-ffac-4656-a409-219f76088d67)
```
로그인에 성공하면 로그인할 때 쓴 이메일을 출력하고 로그인되지 않았을 때는 로그인해주세요 라는 문구가 출력되도록 코드를 짰다.
```
![image](https://github.com/chihyunwon/Kotlin_Null/assets/58906858/7652e03b-5073-469c-8c93-6a5f57fa52fb)
```
로그인되지 않았을 때 (= email이 null일때) null일 때 if를 사용하여 header TextView를 제어하려고 했지만 제어가 되지않고
null이 나오는 모습이다.
```
## 문제 해결방법
![image](https://github.com/chihyunwon/Kotlin_Null/assets/58906858/60bbcb75-c5ab-4de5-8a9a-85e84c1e668d)
```
의외로 해결 방법은 간단했는데 email을 선언하는 과정에서 toString() 메서드를 제거하고 선언해주니 제대로 if문이 작동하여
email이 null 값 일때 xml의 R.id.account의 텍스트를 로그인해주세요로 수정됨을 확인하였다.
```
![image](https://github.com/chihyunwon/Kotlin_Null/assets/58906858/0cd6b3ec-c29d-4472-8548-4780b80a2f73)

