<img width="574" height="282" alt="956e40757abba246d484c072b7d4950" src="https://github.com/user-attachments/assets/4d1b38f8-0e30-4a77-986f-a2d39dd903a1" /><br>
5U机框太矮，所以没法用交换卡转背板流，是通过背板走线去映射三个槽道的背板口，是一一对应的<br>
1-12口是其他厂家开发的，我们的软件只能访问13口之后<br>
蛇形打流的话类似于对接的规则，打到头再返回<br>
有port fwd命令无法在背板口间转发流量<br>
背板流量限制200G<br>
<br>
<br>
port 1/F/20 fwd port 1/B/1<br>
port 1/B/2 fwd port 1/B/3<br>
port 1/B/4 fwd port 1/B/5<br>
port 1/B/6 fwd port 1/B/7<br>
port 1/B/8 fwd port 2/B/1<br>
port 1/B/7 fwd port 1/B/6<br>
port 1/B/5 fwd port 1/B/4<br>
port 1/B/3 fwd port 1/B/2<br>
port 1/B/1 fwd port 1/F/20<br>
<br>
port 2/B/3 fwd port 2/B/4<br>
port 2/B/7 fwd port 2/B/8<br>
port 2/B/2 fwd port 2/B/5<br>
port 2/B/6 fwd port 2/B/6<br>
port 2/B/5 fwd port 2/B/2<br>
port 2/B/1 fwd port 1/B/8<br>
port 2/B/8 fwd port 2/B/7<br>
port 2/B/4 fwd port 2/B/3<br>
<br>
port 3/B/3 fwd port 3/B/4<br>
port 3/B/7 fwd port 3/B/8<br>
port 3/B/1 fwd port 3/B/2<br>
port 3/B/5 fwd port 3/B/6<br>
port 3/B/6 fwd port 3/B/5<br>
port 3/B/2 fwd port 3/B/1 <br>
port 3/B/8 fwd port 3/B/7<br>
port 3/B/4 fwd port 3/B/3<br>
<br>
