# Compressing Scene Dynamics: A Generative Approach

### Shanzhi Yin&dagger;, Zihan Zhang&dagger;, Bolin Chen&dagger;, Shiqi Wang&dagger; and Yan Ye&sect;

#### &dagger; City University of Hong Kong and &sect; Alibaba Group

## Abstruct
This paper proposes to learn generative priors from the motion patterns instead of video contents for generative video compression. The priors are derived from small motion dynamics in common scenes such as swinging trees in the wind and floating boat on the sea. Utilizing such compact motion priors, a novel generative scene dynamics compression framework is built to realize ultra-low bit-rate communication and high-quality reconstruction for diverse scene contents. At the encoder side, motion priors are characterized into compact representations in a dense-to-sparse manner. At the decoder side, the decoded motion priors serve as the trajectory hints for scene dynamics reconstruction via a diffusion-based flowdriven generator. The experimental results illustrate that the proposed method can achieve superior rate-distortion performance and outperform the state-of-the-art conventional video codec Versatile Video Coding (VVC) on scene dynamics sequences. 
<table align="center">
<td align="center">
<img  width="685" alt="Fig 1" src="https://github.com/user-attachments/assets/42d20b4e-453c-4c60-b5a5-09181f14bad9">
</td>
</table>

## Methods
<table align="center">
  <tr>
    <td align="center">
      <img width="679" alt="Fig2" src="https://github.com/user-attachments/assets/488674ab-84ed-4ed5-90ad-550523bf1e13">
      <br />
    </td>
  </tr>
   <td align="center">
     Proposed Dynamics-Codec
    </td>
  </tr>
  
</table>

## Subjective Quality Demos
<table align="center">
  <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>@ 15 kbps</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/32f70d46-efc7-45fe-9371-c23be79a8a25" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/36289414-f4ef-4ce5-8b71-9c8d0f13d385" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/1cddb95f-d5ee-4a1e-9239-6eadd627f11f" width="300" height="300" />
      <br />
    <td align="center">
      <img src="https://github.com/user-attachments/assets/7450b35e-3f14-4521-8664-f1b79890da55" width="300" height="300" />
      <br />
    <td align="center">
      <img src="https://github.com/user-attachments/assets/e261e75c-f4b9-4320-b7b6-8de923a27e11" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/6df83771-cc1b-4ca8-97b1-e8604a50f716" width="300" height="300" />
      <br />
    </td>
  </tr>
   <td align="center">
     Original Sequence
    </td>
    <td align="center">
     VVC Reconstruction
    </td>
  <td align="center">
     ECM Reconstruction
    </td>
  <td align="center">
     DCVC Reconstruction
    </td>
   <td align="center">
   TPSM Reconstruction
  </td>
    <td align="center">
      Dynamics-Codec Reconstruction
    </td>
  </tr>
  
</table>

<table align="center">
  <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>@ 10 kbps</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/9971daa3-a6df-41a0-a63f-8a4261e06e48" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/bd214c0d-c2b5-4df6-8324-cbb50418c0c3" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/f4b16676-28f8-4787-9d35-d18162a5a203" width="300" height="300" />
      <br />
    <td align="center">
      <img src="https://github.com/user-attachments/assets/d786c6b6-08ce-4753-82f1-99aa4e509183" width="300" height="300" />
      <br />
    <td align="center">
      <img src="https://github.com/user-attachments/assets/34235b46-7801-47fd-862c-5932df0255f4" width="300" height="300" />
      <br />
    <td align="center">
      <img src="https://github.com/user-attachments/assets/74835bb4-c481-4ce9-9935-19cf5db03c4c" width="300" height="300" />
      <br />
    </td>
  </tr>
   <td align="center">
     Original Sequence
    </td>
    <td align="center">
     VVC Reconstruction
    </td>
  <td align="center">
     ECM Reconstruction
    </td>
  <td align="center">
     DCVC Reconstruction
    </td>
  <td align="center">
   TPSM Reconstruction
  </td>
    <td align="center">
      Dynamics-Codec Reconstruction
    </td>
  </tr>
  
</table>


<table align="center">
    <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>@ at 7 kbps</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/90819098-5a9a-4d2c-a85a-1ced4ccfcf45" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/a909d62f-0d37-4bfe-8157-61b6f14c8460" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/ac523e72-0e99-4a06-b010-b3a5ff839184" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/02c09e4d-8af0-4cc3-b1c6-4a9ec1543bdf" width="300" height="300" />
      <br />
    </td>
     <td align="center">
      <img src="https://github.com/user-attachments/assets/65dc2c5c-127f-4ad8-aa6b-8053442dfcc7" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/784aced7-6e76-4bf8-95ea-5376b4e9ebbc" width="300" height="300" />
      <br />
    </td>
  </tr>
   <tr>
   <td align="center">
     Original Sequence
    </td>
    <td align="center">
     VVC Reconstruction
    </td>
  <td align="center">
     ECM Reconstruction
    </td>
  <td align="center">
     DCVC Reconstruction
    </td>
     <td align="center">
   TPSM Reconstruction
  </td>
    <td align="center">
      Dynamics-Codec Reconstruction
    </td>
  </tr>
</table>


<table align="center">
    <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>@ 6 kbps</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/2a1df68c-6be6-41d1-9a56-90d7012538a0" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/980f4807-296d-4669-b3c5-aa6ec80617df" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/397a000b-2d39-494e-8bb9-9fe6cad14c12" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/10ba49dc-39ee-4b06-ad20-122882d78cda" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/57608ebd-8336-4498-901b-fcd18a073349" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/8756f6a7-088e-44c4-9bc8-18e63f5fba59" width="300" height="300" />
      <br />
    </td>
   </tr>
   <tr>
   <td align="center">
     Original Sequence
    </td>
    <td align="center">
     VVC Reconstruction
    </td>
  <td align="center">
     ECM Reconstruction
    </td>
  <td align="center">
     DCVC Reconstruction
    </td>
    <td align="center">
   TPSM Reconstruction
  </td>
    <td align="center">
      Dynamics-Codec Reconstruction
    </td>
  </tr>
</table>



<table align="center">
    <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>@ at 5 kbps</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/fed5dc43-2dfb-4f12-b7bd-e7ad3b64b92b" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/0a68f251-07e4-480a-9d15-5b6fe23a9015" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/04958f01-6d06-4f86-b3f5-f89557f6a31c" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/354f28b7-3726-4752-aea4-60bfd626b2da" width="300" height="300" />
      <br />
    </td>
     <td align="center">
      <img src="https://github.com/user-attachments/assets/84d1970b-9902-4be3-adb9-b7c1933164d6" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/ec29a2fb-bf3f-4a25-b605-e36108974f5b" width="300" height="300" />
      <br />
    </td>
  </tr>
   <tr>
   <td align="center">
     Original Sequence
    </td>
    <td align="center">
     VVC Reconstruction
    </td>
  <td align="center">
     ECM Reconstruction
    </td>
  <td align="center">
     DCVC Reconstruction
    </td>
     <td align="center">
   TPSM Reconstruction
  </td>
    <td align="center">
      Dynamics-Codec Reconstruction
    </td>
  </tr>
</table>

## Code Release
Comming soon..

### :e-mail: Contact

If you have any question or collaboration need (research purpose or commercial purpose), please email `shanzhyin3-c@my.cityu.edu.hk`
