# SSL-Pinning

1. 아이폰 단말기 ssh 접속 후 `/var/mobile/Media` 경로에서 `dpkg -i com.nablac0d3.sslkillswitch2_0.14.deb` 명령 수행
    1) `dpkg -i com.nablac0d3.sslkillswitch2_0.14.deb` 명령이 제대로 되지 않는다면
        #1 `apt update`
        #2 `apt install preferenceloder`
        #3 `dpkg -i com.nablac0d3.sslkillswitch2_0.14.deb`
            
            또는 `dpkg -i moe.misty.**sslkillswitch3_1.5.1**+roothide_iphoneos-arm64e.deb`   ← ssl kill switch 3 ver. (iOS 높은 버전인 경우)
            
    2) 압축을 풀어야 하는 경우 압축 풀기 실행
    3) dpkg 미설치인 경우 : `apt-get install dpkg` 명령 실행
    
2. `apt-get install -f` 명령 실행

3. `killall -9 SpringBoard` (또는 `killall -HUP SpringBoard`) 실행

4. 기기 내 설정에서 설치 확인 가능 → 버튼 활성화 + 해당 앱의 식별자(ID) 입력
