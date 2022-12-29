kubeadm init \
--apiserver-advertise-address=192.168.137.100 \
--image-repository registry.aliyuncs.com/google_containers \
--service-cidr=10.96.0.0/12 \
--pod-network-cidr=10.244.0.0/16



kubeadm join 192.168.241.5:6443 --token 6ljrc2.1940il7b5vufr54r \
	--discovery-token-ca-cert-hash sha256:a5233665e0ccbc739bf9372432cd7f5985d384a4d7a740106d1181a62671af6b
