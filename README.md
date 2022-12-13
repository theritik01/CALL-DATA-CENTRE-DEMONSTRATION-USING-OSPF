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
![1](https://user-images.githubusercontent.com/99108259/207248828-a71db3e5-b008-4eeb-b2ab-bf26d5e6b305.jpg)
<h3><b>2. The OSPF protocol successfully configured at router 1.</b></h3>
![2](https://user-images.githubusercontent.com/99108259/207249481-9957fbfc-707d-4ec4-b3d8-a698eeeee772.jpg)
<h3><b>3.	Total addresses, IP address range, current index are shown on CLI of router0. Similarly we can check if the DHCP has been set up or not on other routers too. DHCP request on PC0 is successful.</b></h3>
![3](https://user-images.githubusercontent.com/99108259/207249719-cb0e9431-3b30-4014-9971-7a6c3e5005ff.jpg)
<h3><b>4.	Shows the DNS server (192.168.10.5) at zone1 resolving host names into IP addresses.</b></h3>
![4 1](https://user-images.githubusercontent.com/99108259/207249845-ae40d31d-5e98-4d83-8ef6-a4e2483cc1d3.jpg)
![4 2](https://user-images.githubusercontent.com/99108259/207249876-1b2be32c-5329-42d3-97e9-e31e3075b97a.jpg)
<h3><b>Henceforth, the terminal can also be used to check faster implementations and testing our network by also getting a deep insight of the packets lost and the time it took to achieve the results with the loss percentage.</b></h3>
<h3><b>5.	The following message displays the successful pinging of message packets from PC0(192.168.10.6) to PC2(192.168.10.22) and from PC6(192.168.10.8) to PC5(192.168.10.35)</b></h3>
![5](https://user-images.githubusercontent.com/99108259/207250084-6903dead-52c6-442d-a1ed-127e69c63403.jpg)
