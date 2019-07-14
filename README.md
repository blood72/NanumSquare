# 나눔스퀘어 웹 폰트 (NanumSquare Web Font)

## 소개 (Introduce)

![different-result](https://user-images.githubusercontent.com/24821306/61179623-2d9f2400-a641-11e9-8b82-e81dc0595303.png)

다른 분들이 흔히 쓰는 나눔스퀘어 웹 폰트와 비슷합니다.  
한 가지 차이점은, 첨부된 자료를 사용할 경우 글자가 사라지지 않고 대체됩니다.  
장단점이 존재하는 부분이라 관련 프로젝트에 PR을 넣지 않았습니다.   

It is similar to the NanumSquare web font that people commonly use.  
One difference is that if you use the attached file, the letters will not disappear but will be replaced.  
The pros and cons exist, so I did not put PR into the related project.  



## 문제점 (Problem)

![letters-disappear](https://user-images.githubusercontent.com/24821306/61179485-68ec2380-a63e-11e9-819a-b7880744c984.gif)

글자가 사라진다?  
이는 글자 깨짐 현상을 방지하기 위해 파일 내 글리프\(Glyph\)들을 공백처럼 처리시켜 발생한 문제입니다.  

Letters disappear?  
This is caused by the processing of the glyph in the file like a space to avoid character break.  

![fontdrop-analysis](https://user-images.githubusercontent.com/24821306/61181137-dd35bf80-a65c-11e9-9669-bf68e2daecb9.png)
> Results from analysis in [FontDrop!](https://fontdrop.info/)

해당 글꼴을 분석해보면 위와 같은 결과를 얻을 수 있습니다.  
위쪽 데이터는 공식 홈페이지에서 다운로드 받은 NanumSquareR.ttf이고 아래는 그 변형 결과입니다.  
여기서 글리피 수가 압도적으로 많은 것을 확인할 수 있습니다.  
불필요한 글리피를 삭제함으로써 인덱스매핑도 듬성듬성 건너뛰는 부분이 생긴 것을 확인할 수 있습니다.  

If you analyze the font, you'll get the above results.  
The data above is NanumSquareR.ttf downloaded from the official website and is the result of the modification below.  
You can see that there are an overwhelming number of numGlyphs.  
By deleting unnecessary its, you can see also that index mapping has become a random skip.  


## 참조 (Reference)

NAVER 한글한글 아름답게 - https://hangeul.naver.com  
moonspam's NanumSquare - https://github.com/moonspam/NanumSquare  
FontForge Open Source Font Editor - https://fontforge.github.io  
武蔵システム WOFFコンバータ - https://opentype.jp/woffconv.htm  



## 라이선스 (License)

자세한 사항은 해당 문서를 참조하십시오.

See [LICENSE](LICENSE) for more information.
