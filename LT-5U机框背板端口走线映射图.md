<img width="574" height="282" alt="956e40757abba246d484c072b7d4950" src="https://github.com/user-attachments/assets/4d1b38f8-0e30-4a77-986f-a2d39dd903a1" />
5U机框太矮，所以没法用交换卡转背板流，是通过背板走线去映射三个槽道的背板口，是一一对应的
1-12口是其他厂家开发的，我们的软件只能访问13口zhi
蛇形打流的话类似于对接的规则，打到头再返回


port 1/F/20 fwd port 1/B/1
port 1/B/2 fwd port 1/B/3
port 1/B/4 fwd port 1/B/5
port 1/B/6 fwd port 1/B/7
port 1/B/8 fwd port 2/B/1
port 1/B/7 fwd port 1/B/6
port 1/B/5 fwd port 1/B/4
port 1/B/3 fwd port 1/B/2
port 1/B/1 fwd port 1/F/20

port 2/B/3 fwd port 2/B/4
port 2/B/7 fwd port 2/B/8
port 2/B/2 fwd port 2/B/5
port 2/B/6 fwd port 2/B/6
port 2/B/5 fwd port 2/B/2
port 2/B/1 fwd port 1/B/8
port 2/B/8 fwd port 2/B/7
port 2/B/4 fwd port 2/B/3

port 3/B/3 fwd port 3/B/4
port 3/B/7 fwd port 3/B/8
port 3/B/1 fwd port 3/B/2
port 3/B/5 fwd port 3/B/6
port 3/B/6 fwd port 3/B/5
port 3/B/2 fwd port 3/B/1 
port 3/B/8 fwd port 3/B/7
port 3/B/4 fwd port 3/B/3
