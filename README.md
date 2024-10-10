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
      <b>Sequence 015 at 15 kbps</b>
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
      <img src="https://github.com/user-attachments/assets/0c1f1a42-6831-4f71-a803-291b1f54fd36" width="300" height="300" />
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
      Dynamics-Codec Reconstruction
    </td>
  </tr>
  
</table>

<table align="center">
  <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>Sequence 031 at 10 kbps</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/9dbb0e55-4ecb-4420-8c4c-48048c749ca1" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/50536ce7-04bd-4e31-bbda-d8367f6837a1" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/de35b0d6-73b8-4cd1-a8b5-0e84c6cce5d1" width="300" height="300" />
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
      Dynamics-Codec Reconstruction
    </td>
  </tr>
  
</table>

<table align="center">
  <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>Sequence 006 at 8 kbps</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/0aca478e-252f-42d1-8664-b90a011ee9fc" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/ed68ea78-4346-46e4-b938-22fe7fd8e3d6" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/351d1d88-88b3-4a3e-b080-6669dd421382" width="300" height="300" />
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
      Dynamics-Codec Reconstruction
    </td>
  </tr>
  
</table>


<table align="center">
  <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>Sequence 024 at 7 kbps</b>
    </td>
  </tr>

  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/6d95e03c-e6fa-478b-ba9d-95c75a58f300" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/c94733dd-d200-4704-82bb-479b01e3dd5a" width="300" height="300" />
      <br />
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/2e2e202f-4e7a-440e-997e-e1f67fc629a5" width="300" height="300" />
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
      Dynamics-Codec Reconstruction
    </td>
  
</table>


<table align="center">
    <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>Sequence 029 at 6 kbps</b>
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
      <img src="https://github.com/user-attachments/assets/a9b94fa7-8efa-41bd-9ddc-18e76dbcc573" width="300" height="300" />
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
      Dynamics-Codec Reconstruction
    </td>
    
  </tr>
</table>



<table align="center">
    <tr>
    <td colspan="3" align="center" style="border: none;">
      <b>Sequence 034 at 5 kbps</b>
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
      <img src="https://github.com/user-attachments/assets/fd5baf29-e50a-4544-a358-f165acdf3c08" width="300" height="300" />
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
      Dynamics-Codec Reconstruction
    </td>
    
  </tr>
</table>
