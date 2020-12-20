# Story_Multi_Label_Emotion_Classifier
Pre-training of BERT를 사용한 story text multi label emotion classification 모델.

## Dataset
- [storycommonsense 데이터](https://uwnlp.github.io/storycommonsense/) : Enabling reasoning about the cause and effect of mental state changes of characters in a story.
- 전체 : 19,393 문장
- train : 8,145 문장 
- validation : 3,491 문장
- test : 7,757 문장

## GPU
- Colab

## Task

**INPUT TEXT** 
```
Karen agreed happily. The show was absolutely exhilarating.
```

**OUTPUT**
|joy|anticipation|fear|surprise|anger|sadness|trust|disgust|
|-|-|-|-|-|-|-|-|
|1|1|0|1|0|0|0|0|

## Result
- average f1 score : 0.63

## Example
```
prediction_sample('Jennifer has a big exam tomorrow. She got so stressed, she pulled an all-nighter.')
```
|joy|anticipation|fear|surprise|anger|sadness|trust|disgust|
|-|-|-|-|-|-|-|-|
|0|0|1|0|0|1|0|0|

```
prediction_sample('Karen agreed happily. The show was absolutely exhilarating.') 
```
|joy|anticipation|fear|surprise|anger|sadness|trust|disgust|
|-|-|-|-|-|-|-|-|
|1|1|0|1|0|0|0|0|
