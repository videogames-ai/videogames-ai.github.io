---
layout: page
title:  "Tensorflow.js performance test"
permalink: /Tensorflow-js-performance-test
tags: [tensorflow.js, performance, test, benchmark]
---


<body>
  <!-- ===================================================  -->
<!-- Host Info                                            -->
<!-- ===================================================  -->
<h3> Host Info</h3>
<div id='div-hostinfo'>
  <table id='table-hostinfo' border='1' border-width='5px'>
    <tr>
      <td>GPU</td>
      <td id="host-gpu"></td>

    </tr>
    <tr>
      <td>TF Version</td>
      <td id='host-tfversion'></td>
    </tr>
    <tr>
      <td>TF Backend</td>
      <td id='host-tfbackend'></td>
    </tr>
    <tr>
      <td>WebGL version</td>
      <td id='host-webglversion'></td>
    </tr>
    <tr>
      <td>Force f16 textures</td>
      <td id='host-forcef16'></td>
    </tr>
    <tr>
      <td>Debug Mode</td>
      <td id='host-debug'></td>
    </tr>
  </table>


  
    <canvas id="glcanvas" width="0" height="0">
      <script src="host_info.js"></script>
    </canvas>
  </div>

  <button onclick="StartTest()">Start Test</button>
  <button onclick="StartTest2()">Start Test 2</button>

  <!-- ===================================================  -->
<!-- Test Results                                          -->
<!-- ===================================================  -->
<div id='div-testresults'>
  <table id='table-hostinfo' border='1'>
    <tr>
      <th>Test</th>
      <th>Result</th>
    </tr>
    <tr>
      <td>MatMul</td>
      <td id="tr-matmul"></td>
    </tr>
    <tr>
      <td>Mnist</td>
      <td id="tr-mnist"></td>
    </tr>
  </table>


  <!-- ===================================================  -->
<!-- Output                                         -->
<!-- ===================================================  -->
<h3> Output</h3>


<texarea type="text" id='test-output'>

<script src="main.js"></script>
<script src="tf-tests/matmul.js"></script>
<script src="tf-tests/mnist.js"></script>