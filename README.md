# CALL-DATA-CENTRE-DEMONSTRATION-USING-OSPF
This project briefly explains the concept of OSPF protocol and shows its implementation with a use case scenario. Here the scenario is communication and transmission of data, within the branches of a call center. It also illustrates OSPF protocol’s benefits and possible (if any) issues.
<h1 align="center">ROUTING TABLES</h1>
<table align="center">
  <tr>
    <th>Name of call center branch</th>
    <th>Router number</th>
    <th>Starting address</th>
    <th>Broadcast address</th>
    <th>Subnet Mask
  </tr>
  <tr>
    <td>Dotcom</td>
    <td>R0</td>
    <td>192.168.10.0</td>
    <td>192.168.10.5</td>
    <td> 28 </td>
  </tr>
   <tr>
    <td>Dot2com</td>
    <td>R1</td>
    <td>192.168.10.16</td>
    <td>192.168.10.31</td>
    <td> 28 </td>
  </tr>
   <tr>
    <td>Dot3com</td>
    <td>R2</td>
    <td>192.168.10.32</td>
    <td>192.168.10.47</td>
    <td> 28 </td>
  </tr>
</table>
<table align="center">
<tr>
<th>From Router</th>
<th>To Router</th>
<th>Network ID</th>
</tr>
<tr>
<th>Router0</th>
<th>Router1</th>
<th>10.0.0.0</th>
</tr>
<tr>
<th>Router1</th>
<th>Router2</th>
<th>11.0.0.0</th>
</tr>
<tr>
<th>Router2</th>
<th>Router0</th>
<th>12.0.0.0</th>
</tr>
<tr>
<th>Router1</th>
<th>Router3</th>
<th>13.0.0.0</th>
</tr>
<tr>
<th>Router2</th>
<th>Router4</th>
<th>14.0.0.0</th>
</tr>
<tr>
<th>Router3</th>
<th>Router5</th>
<th>15.0.0.0</th>
</tr>
<tr>
<th>Router4</th>
<th>Router6</th>
<th>16.0.0.0</th>
</tr>
<tr>
<th>Router5</th>
<th>Router7</th>
<th>17.0.0.0</th>
</tr>
<tr>
<th>Router6</th>
<th>Router8</th>
<th>18.0.0.0</th>
</tr>
<tr>
<th>Router7</th>
<th>Router9</th>
<th>19.0.0.0</th>
</tr>
<tr>
<th>Router9</th>
<th>Router8</th>
<th>20.0.0.0</th>
</tr>
<tr>
<th>Router8</th>
<th>Router5</th>
<th>21.0.0.0</th>
</tr>
<tr>
<th>Router6</th>
<th>Router3</th>
<th>22.0.0.0</th>
</tr>
<tr>
<th>Router0</th>
<th>Router3</th>
<th>23.0.0.0</th>
</tr>
<tr>
<th>Router4</th>
<th>Router7</th>
<th>24.0.0.0</th>
</tr>
</table>

<h2>Assignable host address= 14 each</h2>


<h1 align="center"><strong>TESTING & ANALYSIS</strong></h1>
<h3><b>1.	The CLI of router 0 shows the internet address with the subnet mask and broadcast address. Assignment of IP addresses is successful.</b></h3>
![alt text](https://user-images.githubusercontent.com/99108259/207247418-34019523-184d-4e64-8aea-a04ffeb6cb89.jpg "Optional title")

