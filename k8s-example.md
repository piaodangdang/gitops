kubectl create -f https://ghproxy.com/https://raw.githubusercontent.com/lyzhang1999/resource/main/ingress-nginx/ingress-nginx.yaml

kubectl apply -f https://ghproxy.com/https://raw.githubusercontent.com/lyzhang1999/resource/main/metrics/metrics.yaml


kubectl apply -f https://ghproxy.com/https://raw.githubusercontent.com/lyzhang1999/kubernetes-example/main/deploy/database.yaml -n example

kubectl wait --for=condition=Ready pods --all -n example

kubectl patch hpa backend -p '{"spec":{"minReplicas": 3}}' -n example


## 苹果启用root

1 键入或粘贴 /System/Library/CoreServices/Applications/，然后按下回车键 
2 从打开的窗口打开目录实用工具
