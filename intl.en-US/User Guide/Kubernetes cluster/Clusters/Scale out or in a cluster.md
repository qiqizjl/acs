# Scale out or in a cluster {#task_glw_vmg_vdb .task}

In the Container Service console, you can scale out or scale in the worker nodes of a Kubernetes cluster according to your actual business requirements.

**Instructions**

-   Currently, Container Service only supports manually scaling in and out a cluster and does not support auto scaling.
-   Currently, Container Service does not support scaling in and out the master nodes in a cluster.
-   Container Service only supports scaling in the worker nodes that are created when you create the cluster or added after you scale out the cluster. The worker nodes that are added as existing ECS instances when you create the cluster cannot be scaled in.
-   When you scale in a cluster, the worker nodes are removed from the cluster in the order that they are added after you scale out the cluster.

1.   Log on to the [Container Service console](https://partners-intl.console.aliyun.com/#/cs%20%22Container%20Service%20console%22). 
2.   Click Kubernetes \> **Clusters** in the left-side navigation pane. 
3.   Click **Scale Cluster** at the right of the cluster. 

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/6885/4327_en-US.png)

4.   Select **Scale out** or **Scale in** in the Scale field and then configure the number of worker nodes. 

    In this example, scale out the cluster and change the number of worker nodes from one to four.

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/6885/4328_en-US.png)

5.   Enter the logon password of the node. 

    **Note:** Make sure this password is the same as the one you entered when creating the cluster because you have to log on to the Elastic Compute Service \(ECS\) instance to copy the configuration information in the upgrade process.

6.   Click **Submit**. 

After scaling out the cluster, click Kubernetes \> Clusters \> Nodes in the left-side navigation pane. You can view that the number of worker nodes changes from one to four.
