# HCI_crawling
Big Kinds crawling repository for HCL class

# Setting
일단 전북대에서 만든 샘플부터 돌립니다.  
저는 콘다 기반으로 했기 때문에, conda 환경 기준으로 사용방법 씁니다.  
먼저 내 chrome 버전과 맞는 webdriver부터 깔려있다는 전제로 합니다.
webdriver-manager를 설치합니다.

```
 conda install -c conda-forge webdriver-manager 
```

그리구 'cralwer.py' 의 'webdriver.Chrome()' 를 다음과 같이 바꿉니다.

```
self.driver = webdriver.Chrome(ChromeDriverManager().install(), options=options)
```

다 완료되면, 해당 디렉토리로 이동한후

```
python crawler.py 
```

실행하면 됩니다.
