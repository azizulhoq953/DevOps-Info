# DevOps-Error solving
* Kubernetes master Node problem errors solution:

*Kubernetes Error Master Node in Ubuntu Server Version Vm*

> error execution phase wait-control-plane: couldn't initialize a Kubernetes 
> cluster To see the stack trace of this error execute with --v=5 or higher.

* Error Solve In follow Step By Step command:
 
 ``kubeadm reset -f``
 
 >``iptables -F && iptables -t nat -F && iptables -t mangle -F && iptables -X``
 
 >``cat > /etc/docker/daemon.json <<EOF``
 
 *Select all Command:
 `{`
 
  `"exec-opts": ["native.cgroupdriver=systemd"],`
  
  `"log-driver": "json-file",`
  
  `"log-opts": {`
  
   ` "max-size": "100m"`
	
  `},`
  
  `"storage-driver": "overlay2"`
  
 `}`
`EOF`



