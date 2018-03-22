
This sample code shows how to run a task on an object in vSphere. Specifically, it run a  destroy task on one of these object types: VirtualMachine, Datacenter, Folder, HostSystem, ResourcePool, ComputeResource, or ClusterComputeResource.

This sample assumes you are running vSphere version 5.5 or later.

How To Run

In order to run this sample code you must provide five arguments:
[1] The server name or IP address
[2] The user name to log in as
[3] The password to use
[4] The type of object to destroy
[5] The name of the object to destroy

You will need to get the vim25.jar library from the VMware vSphere JDK.  It is in the VMware-vSphere-SDK-5.5.0\vsphere-ws\java\JAXWS\lib directory.

You can run this sample code by downloading the zip file below, unzipping it, and running a command similar to the following:
java -cp vim25.jar com.vmware.scia.general.Destroy ip_or_name user password type name_of_object
java -cp vim25.jar com.vmware.scia.general.Destroy 10.20.30.40 JoeUser JoePasswd VirtualMachine vm1

Output

You will see the output similar to the following when you run the sample:
c:\vmware\sciaproj>./run_samples.sh general.Destroy 10.67.118.172 administrator quiet!word VirtualMachine oldVM
Success
