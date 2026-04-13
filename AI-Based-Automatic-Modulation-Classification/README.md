<div align="center">
  <h1>Hybrid Deep Learning for Automatic Modulation Classification (AMC)</h1>
  <p><i>Leveraging Deep Residual Learning and Temporal Dependencies for 6G Wireless Systems</i></p>
</div>

<hr>

<h2>🚀 Project Overview</h2>
<p>
  This repository implements a high-performance <b>ResNet-LSTM</b> hybrid neural network for <b>Automatic Modulation Classification (AMC)</b>. 
  By processing complex-valued I/Q signals from the <b>RML2016.10b</b> dataset, the model performs signal classification 
  across a wide range of Signal-to-Noise Ratios (SNR). This work is tailored for AI-native communication systems, 
  cognitive radio, and the evolution toward intelligent 6G networks.
</p>

<h3>Key Technical Features</h3>
<ul>
  <li><b>Residual Learning:</b> Integrated skip connections to ensure efficient gradient flow in deep convolutional layers.</li>
  <li><b>Temporal Modeling:</b> Stacked LSTM layers to capture long-term temporal dependencies within signal sequences.</li>
  <li><b>Data Pipeline:</b> Automated I/Q signal reshaping $(2, 128, 1)$ and label binarization for multi-class classification.</li>
</ul>

<hr>

<h2>🏗️ Model Architecture</h2>
<p>The classification pipeline consists of the following stages:</p>
<table width="100%">
  <tr>
    <th align="left">Stage</th>
    <th align="left">Component</th>
    <th align="left">Function</th>
  </tr>
  <tr>
    <td>1</td>
    <td><b>Input</b></td>
    <td>Raw I/Q Signal Vectors $(2 \times 128)$</td>
  </tr>
  <tr>
    <td>2</td>
    <td><b>Feature Extraction</b></td>
    <td>ResNet Blocks (Conv2D + BatchNormalization + Add)</td>
  </tr>
  <tr>
    <td>3</td>
    <td><b>Temporal Analysis</b></td>
    <td>TimeDistributed Flatten + Dual LSTM Layers</td>
  </tr>
  <tr>
    <td>4</td>
    <td><b>Classification</b></td>
    <td>Dense Softmax (10 Modulation Classes)</td>
  </tr>
</table>

<hr>

<h2>🛠️ Tech Stack</h2>
<p align="left">
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/MATLAB-ED1C24?style=for-the-badge&logo=mathworks&logoColor=white" />
</p>

<hr>

<h2>📬 Contact & Connect</h2>
<p>
  <b>Mohamed Mohamed Elsagheer</b><br>
  Assistant Lecturer | Department of Electronics and Communication Engineering<br>
  Faculty of Engineering, Sohag University
</p>

<p>
  <a href="mailto:mohamed.elsagheer@eng.sohag.edu.eg">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/mohamed-elsagheer-51596919a/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
</p>

<hr>
<div align="center">
  <p><i>Advancing autonomous agents and intelligent signal processing for next-generation wireless networks.</i></p>
</div>
