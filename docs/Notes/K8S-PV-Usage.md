

# K8S PV Usage








<div>Work Flow:</div><ol><li>Defined a PVC while creating a Pod.</li><li>Pod assigned to NodeA.</li><li>Kubelet will waiting for Volume Manager to prepare.</li><li>PC Controller will call the poresbonding Volume Plugins to create PV and bind PV with PVC.</li><li>Attach/Detach Controller will mount the volume through the volume plugin.</li><li>Volume Manager tell kubelet the preparation job is done.</li><li>Kubelet start to create pod.</li></ol><br>

