## Part 1.  Deploying your own k3s cluster

#### 1. Get a set of virtual machines for the cluster
![1.1](./images/part_1/1.1.png)

#### 2. Install k3s on all three machines. When installing, do not use the standard Ingress Controller by using the flag --disable=traefik
![1.2](./images/part_1/1.2.png)
![1.2](./images/part_1/1.2.1.png)
![1.3](./images/part_1/1.3.png)

#### 3. Connect the nodes to the cluster using the k3s server command and the -token and --server flags for worker and master nodes respectively. When k3s is installed, the environment variable NODE_TOKEN can be used.
![1.4](./images/part_1/1.4.png)

#### 4. Install the Ingress Controller Nginx instead of the default one. You can use the official nginx-based ingress controller manifest file available on GitHub.
![1.5](./images/part_1/1.5.png)
![1.6](./images/part_1/1.6.png)