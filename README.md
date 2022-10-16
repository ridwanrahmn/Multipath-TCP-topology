# Multipath-TCP-topology


Multipath TCP (MPTCP) adalah metode yang menggunakan beberapa IP address/interface secara simultan dengan dasar TCP biasa yang dimodifikasi. Manfaat dari MPTCP adalah pemanfaatan sumber daya dan throughput yang lebih baik, serta lebih peka terhadap kegagalan.

Simulasi dapat dilakukan dengan menggunakan Mininet-WiFi. Topologi dibuat dengan memanfaatkan miniedit pada Mininet-WiFi sehingga akan lebih mudah. Topologi MPTCP yang dibuat terdiri dari Controller, STA1 (client), AP1, AP2, S5, S6, S7 dan h4. Bentuk topologinya dapat dilihat pada file image-topo-mptcp.jpg.

# Testing


Tes yang dilakukan dalam implementasi topologi ini adalah sebagai berikut:
<br /> 1> Tes throughput : jalankan command **h4 iperf -s** pada h4 lalu **iperf -c 10.0.0.2 --time 60 --interval 2** dari STA1
<br /> 2> Ping : jalankan command **ping 10.0.0.2** dari STA1
<br /> 3> Jalankan keduanya secara bersamaan antara tes throughput dan ping
<br /> 4> Gunakan command **netstat-s** untuk melihat informasi dari tes tersebut
