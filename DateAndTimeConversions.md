# Como diferenciar los formatos fechas en SQLserver

## Formato Fecha sin Hora
<table>
  <tr>
      <th>Query</th><th>Resultado</th>
  </tr>  
    <tr><td>select convert(varchar, getdate(), 1)</td><td>12/30/06</td></tr>
<tr><td>select convert(varchar, getdate(), 2)</td><td>06.12.30</td></tr>
<tr><td>select convert(varchar, getdate(), 3)</td><td>39081</td></tr>
<tr><td>select convert(varchar, getdate(), 4)</td><td>30.12.06</td></tr>
<tr><td>select convert(varchar, getdate(), 5)</td><td>39081</td></tr>
<tr><td>select convert(varchar, getdate(), 6)</td><td>30 Dec 06</td></tr>
<tr><td>select convert(varchar, getdate(), 7)</td><td>Dec 30, 06</td></tr>
<tr><td>select convert(varchar, getdate(), 10)</td><td>12-30-06</td></tr>
<tr><td>select convert(varchar, getdate(), 11)</td><td>11298</td></tr>
<tr><td>select convert(varchar, getdate(), 12)</td><td>61230</td></tr>
<tr><td>select convert(varchar, getdate(), 23)</td><td>39081</td></tr>
<tr><td>select convert(varchar, getdate(), 101)</td><td>12/30/2006</td></tr>
<tr><td>select convert(varchar, getdate(), 102)</td><td>2006.12.30</td></tr>
<tr><td>select convert(varchar, getdate(), 103)</td><td>39081</td></tr>
<tr><td>select convert(varchar, getdate(), 104)</td><td>30.12.2006</td></tr>
<tr><td>select convert(varchar, getdate(), 105)</td><td>39081</td></tr>
<tr><td>select convert(varchar, getdate(), 106)</td><td>30 Dec 2006</td></tr>
<tr><td>select convert(varchar, getdate(), 107)</td><td>Dec 30, 2006</td></tr>
<tr><td>select convert(varchar, getdate(), 110)</td><td>12-30-2006</td></tr>
<tr><td>select convert(varchar, getdate(), 111)</td><td>39081</td></tr>
<tr><td>select convert(varchar, getdate(), 112)</td><td>20061230</td></tr>  
</table>
## Formato Hora
<table>
  <tr>
      <th>Query</th><th>Resultado</th>
  </tr> 
  <tr><td>select convert(varchar, getdate(), 8)</td><td>0.0270138888888889</td></tr>
<tr><td>select convert(varchar, getdate(), 14)</td><td>00:38:54:840</td></tr>
<tr><td>select convert(varchar, getdate(), 24)</td><td>0.0270138888888889</td></tr>
<tr><td>select convert(varchar, getdate(), 108)</td><td>0.0270138888888889</td></tr>
<tr><td>select convert(varchar, getdate(), 114)</td><td>00:38:54:840</td></tr>
</table>
