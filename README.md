# 08-cdots-project

CNN, image recognition study materials
CNN, image recongnition 공부 자료


공부중...

https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html
https://jonathan-hui.medium.com/gan-dcgan-deep-convolutional-generative-adversarial-networks-df855c438f
http://daddynkidsmakers.blogspot.com/2017/02/blog-post_24.html
https://www.youtube.com/watch?v=h7iBpEHGVNc&ab_channel=StanfordUniversitySchoolofEngineeringStanfordUniversitySchoolofEngineering
https://www.youtube.com/watch?v=f0t-OCG79-U
https://www.cs.ryerson.ca/~aharley/vis/conv/flat.html
https://www.superdatascience.com/blogs/the-ultimate-guide-to-convolutional-neural-networks-cnn

어렵다 (이제 다 이해함)

계속 공부중

almost done
아직
하는중
다함
이제 rnn

1. input image (너무 큼. 그래서 작게 만들어주거나, 대강의 느낌을 파악해야함.) 그래서 feature detector로 convolve함.
2. 그렇게 해서 나오는게 feature map(=activation map)
3. 이걸 여러번 해서 feature map을 모으면 그게 하나의 convolutional layer가 됨
4. 그다음 feature map들의 non-linearity을 키우기 위해서 ReLU 함수에 통과 시킴.
5. 그다음에 해야하는건 pooling임 (이거를 하는 이유는 이미지의 텍스쳐, 촬영 거리, 각도 등으로 인한 오차를 최대한 줄이기 위해서임. Max, sum, mean 등의 pooling이 있음. 이거를 수행하면 'spatial variance'를 유지할 수 있음)
6. spatial variance는 중요한게 이미지에서는 픽셀간의 공간적인 상대적 위치가 중요하기 때문임.
7. 하여간 이 pooling layer를 얻어냄.
8. 그다음엔 이 pooling layer들을 각각 flattening 해줄거임. 길게 늘어놓는거임.
9. 그리고 이제 이 flattened layer를 ANN에 넣어주어야 함.
