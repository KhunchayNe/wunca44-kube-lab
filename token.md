Your Kubernetes control-plane has initialized successfully!

To start using your cluster, you need to run the following as a regular user:

  mkdir -p $HOME/.kube
  sudo cp -i /etc/kubernetes/admin.conf $HOME/.kube/config
  sudo chown $(id -u):$(id -g) $HOME/.kube/config

Alternatively, if you are the root user, you can run:

  export KUBECONFIG=/etc/kubernetes/admin.conf

You should now deploy a pod network to the cluster.
Run "kubectl apply -f [podnetwork].yaml" with one of the options listed at:
  https://kubernetes.io/docs/concepts/cluster-administration/addons/

You can now join any number of control-plane nodes by copying certificate authorities
and service account keys on each node and then running the following as root:

  kubeadm join 10.0.2.4:6443 --token v1wg1v.6rei5ppyw14pduv4 \
        --discovery-token-ca-cert-hash sha256:5a5faee332a1d58df93bb200f99b207fb28220f617ce3074bb7aeb0f2143b059 \
        --control-plane

Then you can join any number of worker nodes by running the following on each as root:

kubeadm join 10.0.2.4:6443 --token v1wg1v.6rei5ppyw14pduv4 \
        --discovery-token-ca-cert-hash sha256:5a5faee332a1d58df93bb200f99b207fb28220f617ce3074bb7aeb0f2143b059



    sudo kubeadm join 10.0.2.4:6443 --token v1wg1v.6rei5ppyw14pduv4 \
        --discovery-token-ca-cert-hash sha256:5a5faee332a1d58df93bb200f99b207fb28220f617ce3074bb7aeb0f2143b059



//dashboard token


eyJhbGciOiJSUzI1NiIsImtpZCI6IkFjZUl3UkJaMjVzLS1zREdRdG9LUGU0dlhENUx2Z3pSOGJWUFAwaWtwaXcifQ.eyJhdWQiOlsiaHR0cHM6Ly9rdWJlcm5ldGVzLmRlZmF1bHQuc3ZjLmNsdXN0ZXIubG9jYWwiXSwiZXhwIjoxNzM4ODMwNTg3LCJpYXQiOjE3Mzg4MjY5ODcsImlzcyI6Imh0dHBzOi8va3ViZXJuZXRlcy5kZWZhdWx0LnN2Yy5jbHVzdGVyLmxvY2FsIiwianRpIjoiNjA5NzNmYTQtNmVjZC00ZDEzLTljZGYtNzY2Y2RjZTBiN2NkIiwia3ViZXJuZXRlcy5pbyI6eyJuYW1lc3BhY2UiOiJrdWJlcm5ldGVzLWRhc2hib2FyZCIsInNlcnZpY2VhY2NvdW50Ijp7Im5hbWUiOiJhZG1pbi11c2VyIiwidWlkIjoiMmE3MDBiYmUtZTNhYy00NmU1LTg4NzgtYmFmZjA0NWRmMDhhIn19LCJuYmYiOjE3Mzg4MjY5ODcsInN1YiI6InN5c3RlbTpzZXJ2aWNlYWNjb3VudDprdWJlcm5ldGVzLWRhc2hib2FyZDphZG1pbi11c2VyIn0.X2MFT3bDmSUu31OgOHIZIiNBRMVlj6hqIFfq_HuwOLQYLUnqdjp1vrILSIT-JfRPW5gTi6cMcX0T1qCFORWPMatXYkhVx5WQzuWnfAyF4WiBpb9MIEwAV9w6lsmb8b21g0OQZOcCczsbyEqembYj1-k4bpFi5ysniuJJUREnEv1UijGzj_sRGqZlZHCPPi-DaTT7E_v-9C8VW13nsrlh44KHUXANSrhjQWK2LwLO9TaWNPyd44QcbLKixavOKthDud7p4TQVFjC3kia9mcL8YdtBwjzHsn43nmy0DK8XdLnT6SWWOM8iaNlYZ_ClrR7xGFE1w1bCThJIDnytvZ6txw