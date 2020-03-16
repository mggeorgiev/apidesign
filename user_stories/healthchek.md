<p><b>Description:</b></p>
<p>
As a DAIS Backend (BE) Application, <br>
I want to check if the distributed anti-fraud system is ready to accept request for /score and /action,</br>
so that we can test before sending real data or verify service restoration.
</p>

<ul>
<li>when the BE GETs {{ address }}/healthCheck</li>
<li>then ARGOS will reply with:</li>
  <ul>
      <li>Code 200 success - healthCheck OK</li>
      <li>Code 503 - This node is not ready to receive /score and /actions requests</li>
  </ul>
</ul>

<p></p>

<p>Resources:</p>
<p>Swagger: /healthCheck:</p>
