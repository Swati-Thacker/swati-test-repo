# Coherence Operator Documentation

Oracle enables organizations using Coherence to move their clusters into the cloud. By supporting industry standards, such as Docker and Kubernetes, Oracle facilitates running Coherence on cloud-neutral infrastructure. In addition, Oracle provides an open-source Coherence Operator (“the operator”), which implements features to assist with deploying and managing Coherence clusters in a Kubernetes environment. You can:
 - Run Coherence within the de facto standard Kubernetes container orchestration framework, using Docker containers for the members of a Coherence cluster.
  - Use popular industry standard tools such as Grafana, ELK (or more specifically the EFK stack including Fluentd), and Prometheus to monitor the performance, logs and and health of your clusters.
  - Flexibly override and customize cluster configuration.
  - Scale the Coherence deployment.
  - Use Coherence*Extend to access your cluster with a variety of clients.
  - Use Kubernetes Zone information to ensure data stored in Coherence is resilient to loss of a Zone. Coherence goes to great efforts to ensure data is safe across processes, machines, racks and sites. When Coherence is deployed to Kubernetes with the Coherence Operator, data will be spread across zones to ensure this underlying principle is supported; thus by default, loss of any zone is a tolerated failure mode. This is reflected in the StatusHA value (SITE-SAFE) for partitioned services, in addition to the member level site information that is equivalent to the kubernetes zone label on the associated pod.
  - Start clusters based on declarative startup parameters and desired states.
  - Use Kubernetes persistent volumes when using Coherence’s disk-based storage features Elastic Data or Persistence.
  - Deploy custom code for your EntryProcessor classes and other server-side Coherence constructs.
  
 The fastest way to experience the operator is to follow the Quick Start guide, or try out the samples.
