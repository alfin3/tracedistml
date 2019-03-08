## tracedistml

Initial iterations of distributed approaches to machine learning are being implemented by major companies to address the need for decreasing latencies in real-time applications and processing large amounts of data, in some cases locally. 

Two common considerations are: i) which parts of a computation to distribute and reduce, and ii) how to minimize communication latencies between nodes.

**These considerations pose an optimization problem in the “infrastructure vs. model architecture” search space.** 

To traverse this search space, we need to:
1) quickly iterate across infrastructures and model architectures, and
2) measure the “fit” between an infrastructure and a model architecture.

Towards this goal, as an Insight Fellow, I built: 
1) a one-step provisioning of on-premises capable k8s infrastructures to streamline infrastructure experimentation, and
2) a tool for OpenTracing instrumentation to measure latencies of model construction to guide optimization of real-time systems that require output “freshness” and rapid A/B testing, such as real-time recommendation systems.

## tracedistml/infrastructure

An example of infrastructure provisioning:

![infra_example](https://github.com/alfin3/tracedistml/blob/master/images/infra_image.jpg)


## tracedistml/tracing-ml

A example of OpenTracing instrumentation to measure latencies of model construction:

![latencies_explorer](https://github.com/alfin3/tracedistml/blob/master/images/latencies_explorer.jpg)
