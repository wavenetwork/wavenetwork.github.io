## wavenet 사용 매뉴얼 (TESTING)

```
[>> English-version](index-eng.md)
```

---

### 소개

<img src="wavenet-transmitter.png" width=200px />

요걸로, 17~19kHz 까지 주파수를 선택해서 발신. 발신기.

<img src="wavenet-receiver.png" width=200px />

요걸로, 17~19kHz 까지 주파수를 선택해서 수신. 수신기.
이때, 원하는 주파수만을 강조하기 위해, 다른 주파수 대역의 소리의 크기를 죽이는 필터를 사용하는데.
high pass filter 가 동일 주파수에 4개, low pass filter 가 동일 주파수에 4개 사용됨. (bandpass filter 4개라고 말해도 되공...)
이 두 필터의 중심 주파수를 수신하고자 하는 주파수의 주변에 배치해서.. 원하는 주파수를 포함하는 특정 밴드(band)의 소리만을 듣는다.

이 밴드의 폭을 100Hz에서 2.1kHz 까지, 좁게 혹은 넓게 설정할 수 있다.

이렇게 하는 이유는, 필터의 효과가 사실은 원하는 주파수 대역에도 신호감쇄의 효과를 미치기 때문에, 100Hz 처럼, 정확하게 신호를 잡아내려고 하면, 그만큼 들리는 신호의 크기도 작아지는 효과가 있기 때문에,
바꿔보면서, 테스트해볼 필요가 있다고 생각했기 때문임.

<https://en.wikipedia.org/wiki/Bandwidth_(signal_processing)#X-dB_bandwidth> 의 그림 참고!

---

### 설치 단계 (1) - MobMuplat 설치

---

<a href="https://geo.itunes.apple.com/us/app/mobmuplat/id597679399?mt=8" style="display:inline-block;overflow:hidden;background:url(http://linkmaker.itunes.apple.com/images/badges/en-us/badge_appstore-lrg.svg) no-repeat;width:165px;height:40px;"></a>

<a href="https://play.google.com/store/apps/details?id=com.iglesiaintermedia.mobmuplat">
<img alt="Get it on Google Play" src="https://developer.android.com/images/brand/en_generic_rgb_wo_45.png" />
</a>

**단계 2 진행전 설치 완료 필수!**

---

### 설치 단계 (2) - 따라하기, 말로만~

1. 클릭하여 다운로드 <http://wavenetwork.github.io/wavenet.zip>
2. 다운로드 된거 (wavenet.zip), 클릭하여 열기. 이때, MubMuPlat으로 열기를 선택!
3. 압축 풀려서 잘 설치되었다는 메세지 확인.
4. 좌측 상단의 i 모양 아이콘 클릭
5. 나타난 목록 중, wavenet-transmitter.mmp(또는, wavenet-receiver.mmp)란 파일을 클릭
6. 가운데 동그라미 동글동글을 누르면, 사운드가 발사됨.

---

### 설치 단계 (2) - 따라하기, 그림예시랑 같이, @.@!

* 클릭하여 다운로드 <http://wavenetwork.github.io/wavenet.zip>

<img src="03.png" width=200px />

* 다운로드 된거 (wavenet.zip), 클릭하여 열기. 이때, MubMuPlat으로 열기를 선택!

<img src="04.png" width=200px />
<img src="06.png" width=200px />
<img src="07.png" width=200px />

* 압축 풀려서 잘 설치되었다는 메세지 확인.

<img src="08.png" width=200px />

* 좌측 상단의 i 모양 아이콘 클릭

<img src="09.png" width=200px />

* 나타난 목록 중, wavenet-transmitter.mmp(또는, wavenet-receiver.mmp)란 파일을 클릭

<img src="10.png" width=200px />

* 발신기 앱의 가운데 버튼을 누르면, 신호가 발사됨.

<img src="11.png" width=200px />

* 수신기 앱의 가운데 버튼에 빨간 불이 켜지면, 신호가 수신된 것임.

<img src="11.png" width=200px />

---

- Git repository : <https://github.com/wavenetwork/wavenetwork.github.io>

---