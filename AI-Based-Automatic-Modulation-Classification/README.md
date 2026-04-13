<div align="center">
  <h1>ResNet-LSTM for Automatic Modulation Recognition (AMR)</h1>
  <p><i>Leveraging Deep Residual Learning and Temporal Dependencies for 6G Wireless Systems</i></p>
</div>

<hr>

<h2>🚀 Project Overview</h2>
<p>
  This repository implements a high-performance <b>ResNet-LSTM</b> hybrid neural network for Automatic Modulation Recognition (AMR). 
  By processing complex-valued I/Q signals from the <b>RML2016.10b</b> dataset, the model identifies modulation schemes 
  across a wide range of Signal-to-Noise Ratios (SNR). This research is tailored for AI-native communication systems and 
  semantic networking frameworks.
</p>

<h3>Key Technical Features</h3>
<ul>
  <li><b>Residual Learning:</b> Integrated skip connections to ensure efficient gradient flow in deep convolutional layers.</li>
  <li><b>Temporal Modeling:</b> Stacked LSTM layers to capture long-term dependencies within signal sequences.</li>
  <li><b>Data Pipeline:</b> Automated I/Q signal reshaping $(2, 128, 1)$ and label binarization.</li>
</ul>

<hr>

<h2>🏗️ Model Architecture</h2>
<p>The pipeline consists of the following stages:</p>
<table width="100%">
  <tr>
    <th>Stage</th>
    <th>Component</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>1</td>
    <td><b>Input</b></td>
    <td>Raw I/Q Signal Vectors $(2 \times 128)$</td>
  </tr>
  <tr>
    <td>2</td>
    <td><b>Spatial Blocks</b></td>
    <td>ResNet Blocks (Conv2D + BatchNormalization + Add)</td>
  </tr>
  <tr>
    <td>3</td>
    <td><b>Recurrent Blocks</b></td>
    <td>TimeDistributed Flatten + Dual LSTM Layers</td>
  </tr>
  <tr>
    <td>4</td>
    <td><b>Output</b></td>
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
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
</p>

<hr>

<h2>📬 Contact & Connect</h2>
<p>
  <b>Mohamed El Sagheer</b><br>
  Assistant Lecturer | Department of Nursing Administration<br>
  Faculty of Nursing, Sohag University
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
  <p><i>Contributing to the development of autonomous agents and goal-oriented communication.</i></p>
</div>
