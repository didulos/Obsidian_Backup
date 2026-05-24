---

type: term

category: [Generative-AI, Deep-Learning]

status: seed

---

## 정의

확산 모델(Diffusion Model)은 데이터에 점진적으로 노이즈를 더하는 forward process와 노이즈로부터 원본 데이터를 복원하는 reverse process를 학습하는 생성 모델이다. 이 과정을 통해 random noise에서 시작하여 새로운 데이터를 생성할 수 있다.

## 왜 중요한가

확산 모델은 DALL-E, Stable Diffusion 등 최신 이미지 생성 AI의 핵심 기술이며, [[GAN]](생성적 대립 신경망)보다 학습이 안정적이고 다양한 고품질 콘텐츠를 생성할 수 있다.

## 관련 개념

- 상위 개념: [[Generative-Model]](생성 모델)

- 하위 개념: [[DDPM]](Denoising Diffusion Probabilistic Models), [[Latent-Diffusion]](잠재 확산 모델)

- 연관 개념: [[Denoising]](노이즈 제거), [[Score-Matching]](스코어 매칭), [[Text-to-Image]](텍스트-이미지 생성)

## 비유로 이해하기

흐릿한 사진을 점점 더 흐릿하게 만들다가(forward), 다시 선명하게 복원하는 법을 배우는 것(reverse). 충분히 학습하면 아예 새로운 흐릿한 사진에서 시작해도 선명한 사진을 만들 수 있다.

## 실제 사용 예시

Stable Diffusion에서 "파란 눈을 가진 고양이" 프롬프트로 이미지를 생성할 때, 모델은 무작위 노이즈에서 시작하여 수십 단계의 denoising을 거쳐 최종 이미지를 생성한다.