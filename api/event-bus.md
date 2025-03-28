<p>
Packages:
</p>
<ul>
<li>
<a href="#argoproj.io%2fv1alpha1">argoproj.io/v1alpha1</a>
</li>
</ul>
<h2 id="argoproj.io/v1alpha1">
argoproj.io/v1alpha1
</h2>
<p>
<p>
Package v1alpha1 is the v1alpha1 version of the API.
</p>
</p>
Resource Types:
<ul>
</ul>
<h3 id="argoproj.io/v1alpha1.AuthStrategy">
AuthStrategy (<code>string</code> alias)
</p>
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.NATSConfig">NATSConfig</a>,
<a href="#argoproj.io/v1alpha1.NativeStrategy">NativeStrategy</a>)
</p>
<p>
<p>
AuthStrategy is the auth strategy of native nats installaion
</p>
</p>
<h3 id="argoproj.io/v1alpha1.BusConfig">
BusConfig
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBusStatus">EventBusStatus</a>)
</p>
<p>
<p>
BusConfig has the finalized configuration for EventBus
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>nats</code></br> <em> <a href="#argoproj.io/v1alpha1.NATSConfig">
NATSConfig </a> </em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
<tr>
<td>
<code>jetstream</code></br> <em>
<a href="#argoproj.io/v1alpha1.JetStreamConfig"> JetStreamConfig </a>
</em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ContainerTemplate">
ContainerTemplate
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.JetStreamBus">JetStreamBus</a>,
<a href="#argoproj.io/v1alpha1.NativeStrategy">NativeStrategy</a>)
</p>
<p>
<p>
ContainerTemplate defines customized spec for a container
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>resources</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#resourcerequirements-v1-core">
Kubernetes core/v1.ResourceRequirements </a> </em>
</td>
<td>
</td>
</tr>
<tr>
<td>
<code>imagePullPolicy</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#pullpolicy-v1-core">
Kubernetes core/v1.PullPolicy </a> </em>
</td>
<td>
</td>
</tr>
<tr>
<td>
<code>securityContext</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#securitycontext-v1-core">
Kubernetes core/v1.SecurityContext </a> </em>
</td>
<td>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.EventBus">
EventBus
</h3>
<p>
<p>
EventBus is the definition of a eventbus resource
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>metadata</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#objectmeta-v1-meta">
Kubernetes meta/v1.ObjectMeta </a> </em>
</td>
<td>
Refer to the Kubernetes API documentation for the fields of the
<code>metadata</code> field.
</td>
</tr>
<tr>
<td>
<code>spec</code></br> <em>
<a href="#argoproj.io/v1alpha1.EventBusSpec"> EventBusSpec </a> </em>
</td>
<td>
<br/> <br/>
<table>
<tr>
<td>
<code>nats</code></br> <em> <a href="#argoproj.io/v1alpha1.NATSBus">
NATSBus </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
NATS eventbus
</p>
</td>
</tr>
<tr>
<td>
<code>jetstream</code></br> <em>
<a href="#argoproj.io/v1alpha1.JetStreamBus"> JetStreamBus </a> </em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
</table>
</td>
</tr>
<tr>
<td>
<code>status</code></br> <em>
<a href="#argoproj.io/v1alpha1.EventBusStatus"> EventBusStatus </a>
</em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.EventBusSpec">
EventBusSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBus">EventBus</a>)
</p>
<p>
<p>
EventBusSpec refers to specification of eventbus resource
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>nats</code></br> <em> <a href="#argoproj.io/v1alpha1.NATSBus">
NATSBus </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
NATS eventbus
</p>
</td>
</tr>
<tr>
<td>
<code>jetstream</code></br> <em>
<a href="#argoproj.io/v1alpha1.JetStreamBus"> JetStreamBus </a> </em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.EventBusStatus">
EventBusStatus
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBus">EventBus</a>)
</p>
<p>
<p>
EventBusStatus holds the status of the eventbus resource
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>Status</code></br> <em>
github.com/argoproj/argo-events/pkg/apis/common.Status </em>
</td>
<td>
<p>
(Members of <code>Status</code> are embedded into this type.)
</p>
</td>
</tr>
<tr>
<td>
<code>config</code></br> <em> <a href="#argoproj.io/v1alpha1.BusConfig">
BusConfig </a> </em>
</td>
<td>
<p>
Config holds the fininalized configuration of EventBus
</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.JetStreamAuth">
JetStreamAuth
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.JetStreamConfig">JetStreamConfig</a>)
</p>
<p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>token</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#secretkeyselector-v1-core">
Kubernetes core/v1.SecretKeySelector </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
Secret for auth token
</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.JetStreamBus">
JetStreamBus
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBusSpec">EventBusSpec</a>)
</p>
<p>
<p>
JetStreamBus holds the JetStream EventBus information
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>version</code></br> <em> string </em>
</td>
<td>
<p>
JetStream version, such as “2.7.3”
</p>
</td>
</tr>
<tr>
<td>
<code>replicas</code></br> <em> int32 </em>
</td>
<td>
<p>
Redis StatefulSet size
</p>
</td>
</tr>
<tr>
<td>
<code>containerTemplate</code></br> <em>
<a href="#argoproj.io/v1alpha1.ContainerTemplate"> ContainerTemplate
</a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
ContainerTemplate contains customized spec for Nats JetStream container
</p>
</td>
</tr>
<tr>
<td>
<code>reloaderContainerTemplate</code></br> <em>
<a href="#argoproj.io/v1alpha1.ContainerTemplate"> ContainerTemplate
</a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
ReloaderContainerTemplate contains customized spec for config reloader
container
</p>
</td>
</tr>
<tr>
<td>
<code>metricsContainerTemplate</code></br> <em>
<a href="#argoproj.io/v1alpha1.ContainerTemplate"> ContainerTemplate
</a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
MetricsContainerTemplate contains customized spec for metrics container
</p>
</td>
</tr>
<tr>
<td>
<code>persistence</code></br> <em>
<a href="#argoproj.io/v1alpha1.PersistenceStrategy"> PersistenceStrategy
</a> </em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
<tr>
<td>
<code>metadata</code></br> <em>
github.com/argoproj/argo-events/pkg/apis/common.Metadata </em>
</td>
<td>
<p>
Metadata sets the pods’s metadata, i.e. annotations and labels
</p>
</td>
</tr>
<tr>
<td>
<code>nodeSelector</code></br> <em> map\[string\]string </em>
</td>
<td>
<em>(Optional)</em>
<p>
NodeSelector is a selector which must be true for the pod to fit on a
node. Selector which must match a node’s labels for the pod to be
scheduled on that node. More info:
<a href="https://kubernetes.io/docs/concepts/configuration/assign-pod-node/">https://kubernetes.io/docs/concepts/configuration/assign-pod-node/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>tolerations</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#toleration-v1-core">
\[\]Kubernetes core/v1.Toleration </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
If specified, the pod’s tolerations.
</p>
</td>
</tr>
<tr>
<td>
<code>securityContext</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#podsecuritycontext-v1-core">
Kubernetes core/v1.PodSecurityContext </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
SecurityContext holds pod-level security attributes and common container
settings. Optional: Defaults to empty. See type description for default
values of each field.
</p>
</td>
</tr>
<tr>
<td>
<code>imagePullSecrets</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#localobjectreference-v1-core">
\[\]Kubernetes core/v1.LocalObjectReference </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
ImagePullSecrets is an optional list of references to secrets in the
same namespace to use for pulling any of the images used by this
PodSpec. If specified, these secrets will be passed to individual puller
implementations for them to use. For example, in the case of docker,
only DockerConfig type secrets are honored. More info:
<a href="https://kubernetes.io/docs/concepts/containers/images#specifying-imagepullsecrets-on-a-pod">https://kubernetes.io/docs/concepts/containers/images#specifying-imagepullsecrets-on-a-pod</a>
</p>
</td>
</tr>
<tr>
<td>
<code>priorityClassName</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
If specified, indicates the Redis pod’s priority. “system-node-critical”
and “system-cluster-critical” are two special keywords which indicate
the highest priorities with the former being the highest priority. Any
other name must be defined by creating a PriorityClass object with that
name. If not specified, the pod priority will be default or zero if
there is no default. More info:
<a href="https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/">https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>priority</code></br> <em> int32 </em>
</td>
<td>
<em>(Optional)</em>
<p>
The priority value. Various system components use this field to find the
priority of the Redis pod. When Priority Admission Controller is
enabled, it prevents users from setting this field. The admission
controller populates this field from PriorityClassName. The higher the
value, the higher the priority. More info:
<a href="https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/">https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>affinity</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#affinity-v1-core">
Kubernetes core/v1.Affinity </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
The pod’s scheduling constraints More info:
<a href="https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/">https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>serviceAccountName</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
ServiceAccountName to apply to the StatefulSet
</p>
</td>
</tr>
<tr>
<td>
<code>settings</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
JetStream configuration, if not specified, global settings in
controller-config will be used. See
<a href="https://docs.nats.io/running-a-nats-service/configuration#jetstream">https://docs.nats.io/running-a-nats-service/configuration#jetstream</a>.
Only configure “max_memory_store” or “max_file_store”, do not set
“store_dir” as it has been hardcoded.
</p>
</td>
</tr>
<tr>
<td>
<code>startArgs</code></br> <em> \[\]string </em>
</td>
<td>
<em>(Optional)</em>
<p>
Optional arguments to start nats-server. For example, “-D” to enable
debugging output, “-DV” to enable debugging and tracing. Check
<a href="https://docs.nats.io/">https://docs.nats.io/</a> for all the
available arguments.
</p>
</td>
</tr>
<tr>
<td>
<code>streamConfig</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
Optional configuration for the streams to be created in this JetStream
service, if specified, it will be merged with the default configuration
in controller-config. It accepts a YAML format configuration, available
fields include, “maxBytes”, “maxMsgs”, “maxAge” (e.g. 72h), “replicas”
(1, 3, 5), “duplicates” (e.g. 5m).
</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.JetStreamConfig">
JetStreamConfig
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.BusConfig">BusConfig</a>)
</p>
<p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>url</code></br> <em> string </em>
</td>
<td>
<p>
JetStream (Nats) URL
</p>
</td>
</tr>
<tr>
<td>
<code>auth</code></br> <em>
<a href="#argoproj.io/v1alpha1.JetStreamAuth"> JetStreamAuth </a> </em>
</td>
<td>
</td>
</tr>
<tr>
<td>
<code>streamConfig</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.NATSBus">
NATSBus
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.EventBusSpec">EventBusSpec</a>)
</p>
<p>
<p>
NATSBus holds the NATS eventbus information
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>native</code></br> <em>
<a href="#argoproj.io/v1alpha1.NativeStrategy"> NativeStrategy </a>
</em>
</td>
<td>
<p>
Native means to bring up a native NATS service
</p>
</td>
</tr>
<tr>
<td>
<code>exotic</code></br> <em>
<a href="#argoproj.io/v1alpha1.NATSConfig"> NATSConfig </a> </em>
</td>
<td>
<p>
Exotic holds an exotic NATS config
</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.NATSConfig">
NATSConfig
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.BusConfig">BusConfig</a>,
<a href="#argoproj.io/v1alpha1.NATSBus">NATSBus</a>)
</p>
<p>
<p>
NATSConfig holds the config of NATS
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>url</code></br> <em> string </em>
</td>
<td>
<p>
NATS streaming url
</p>
</td>
</tr>
<tr>
<td>
<code>clusterID</code></br> <em> string </em>
</td>
<td>
<p>
Cluster ID for nats streaming
</p>
</td>
</tr>
<tr>
<td>
<code>auth</code></br> <em>
<a href="#argoproj.io/v1alpha1.AuthStrategy"> AuthStrategy </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
Auth strategy, default to AuthStrategyNone
</p>
</td>
</tr>
<tr>
<td>
<code>accessSecret</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#secretkeyselector-v1-core">
Kubernetes core/v1.SecretKeySelector </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
Secret for auth
</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.NativeStrategy">
NativeStrategy
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.NATSBus">NATSBus</a>)
</p>
<p>
<p>
NativeStrategy indicates to install a native NATS service
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>replicas</code></br> <em> int32 </em>
</td>
<td>
<p>
Size is the NATS StatefulSet size
</p>
</td>
</tr>
<tr>
<td>
<code>auth</code></br> <em>
<a href="#argoproj.io/v1alpha1.AuthStrategy"> AuthStrategy </a> </em>
</td>
<td>
</td>
</tr>
<tr>
<td>
<code>persistence</code></br> <em>
<a href="#argoproj.io/v1alpha1.PersistenceStrategy"> PersistenceStrategy
</a> </em>
</td>
<td>
<em>(Optional)</em>
</td>
</tr>
<tr>
<td>
<code>containerTemplate</code></br> <em>
<a href="#argoproj.io/v1alpha1.ContainerTemplate"> ContainerTemplate
</a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
ContainerTemplate contains customized spec for NATS container
</p>
</td>
</tr>
<tr>
<td>
<code>metricsContainerTemplate</code></br> <em>
<a href="#argoproj.io/v1alpha1.ContainerTemplate"> ContainerTemplate
</a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
MetricsContainerTemplate contains customized spec for metrics container
</p>
</td>
</tr>
<tr>
<td>
<code>nodeSelector</code></br> <em> map\[string\]string </em>
</td>
<td>
<em>(Optional)</em>
<p>
NodeSelector is a selector which must be true for the pod to fit on a
node. Selector which must match a node’s labels for the pod to be
scheduled on that node. More info:
<a href="https://kubernetes.io/docs/concepts/configuration/assign-pod-node/">https://kubernetes.io/docs/concepts/configuration/assign-pod-node/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>tolerations</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#toleration-v1-core">
\[\]Kubernetes core/v1.Toleration </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
If specified, the pod’s tolerations.
</p>
</td>
</tr>
<tr>
<td>
<code>metadata</code></br> <em>
github.com/argoproj/argo-events/pkg/apis/common.Metadata </em>
</td>
<td>
<p>
Metadata sets the pods’s metadata, i.e. annotations and labels
</p>
</td>
</tr>
<tr>
<td>
<code>securityContext</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#podsecuritycontext-v1-core">
Kubernetes core/v1.PodSecurityContext </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
SecurityContext holds pod-level security attributes and common container
settings. Optional: Defaults to empty. See type description for default
values of each field.
</p>
</td>
</tr>
<tr>
<td>
<code>maxAge</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
Max Age of existing messages, i.e. “72h”, “4h35m”
</p>
</td>
</tr>
<tr>
<td>
<code>imagePullSecrets</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#localobjectreference-v1-core">
\[\]Kubernetes core/v1.LocalObjectReference </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
ImagePullSecrets is an optional list of references to secrets in the
same namespace to use for pulling any of the images used by this
PodSpec. If specified, these secrets will be passed to individual puller
implementations for them to use. For example, in the case of docker,
only DockerConfig type secrets are honored. More info:
<a href="https://kubernetes.io/docs/concepts/containers/images#specifying-imagepullsecrets-on-a-pod">https://kubernetes.io/docs/concepts/containers/images#specifying-imagepullsecrets-on-a-pod</a>
</p>
</td>
</tr>
<tr>
<td>
<code>serviceAccountName</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
ServiceAccountName to apply to NATS StatefulSet
</p>
</td>
</tr>
<tr>
<td>
<code>priorityClassName</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
If specified, indicates the EventSource pod’s priority.
“system-node-critical” and “system-cluster-critical” are two special
keywords which indicate the highest priorities with the former being the
highest priority. Any other name must be defined by creating a
PriorityClass object with that name. If not specified, the pod priority
will be default or zero if there is no default. More info:
<a href="https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/">https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>priority</code></br> <em> int32 </em>
</td>
<td>
<em>(Optional)</em>
<p>
The priority value. Various system components use this field to find the
priority of the EventSource pod. When Priority Admission Controller is
enabled, it prevents users from setting this field. The admission
controller populates this field from PriorityClassName. The higher the
value, the higher the priority. More info:
<a href="https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/">https://kubernetes.io/docs/concepts/configuration/pod-priority-preemption/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>affinity</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#affinity-v1-core">
Kubernetes core/v1.Affinity </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
The pod’s scheduling constraints More info:
<a href="https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/">https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/</a>
</p>
</td>
</tr>
<tr>
<td>
<code>maxMsgs</code></br> <em> uint64 </em>
</td>
<td>
<p>
Maximum number of messages per channel, 0 means unlimited. Defaults to
1000000
</p>
</td>
</tr>
<tr>
<td>
<code>maxBytes</code></br> <em> string </em>
</td>
<td>
<p>
Total size of messages per channel, 0 means unlimited. Defaults to 1GB
</p>
</td>
</tr>
<tr>
<td>
<code>maxSubs</code></br> <em> uint64 </em>
</td>
<td>
<p>
Maximum number of subscriptions per channel, 0 means unlimited. Defaults
to 1000
</p>
</td>
</tr>
<tr>
<td>
<code>maxPayload</code></br> <em> string </em>
</td>
<td>
<p>
Maximum number of bytes in a message payload, 0 means unlimited.
Defaults to 1MB
</p>
</td>
</tr>
<tr>
<td>
<code>raftHeartbeatTimeout</code></br> <em> string </em>
</td>
<td>
<p>
Specifies the time in follower state without a leader before attempting
an election, i.e. “72h”, “4h35m”. Defaults to 2s
</p>
</td>
</tr>
<tr>
<td>
<code>raftElectionTimeout</code></br> <em> string </em>
</td>
<td>
<p>
Specifies the time in candidate state without a leader before attempting
an election, i.e. “72h”, “4h35m”. Defaults to 2s
</p>
</td>
</tr>
<tr>
<td>
<code>raftLeaseTimeout</code></br> <em> string </em>
</td>
<td>
<p>
Specifies how long a leader waits without being able to contact a quorum
of nodes before stepping down as leader, i.e. “72h”, “4h35m”. Defaults
to 1s
</p>
</td>
</tr>
<tr>
<td>
<code>raftCommitTimeout</code></br> <em> string </em>
</td>
<td>
<p>
Specifies the time without an Apply() operation before sending an
heartbeat to ensure timely commit, i.e. “72h”, “4h35m”. Defaults to
100ms
</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.PersistenceStrategy">
PersistenceStrategy
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.JetStreamBus">JetStreamBus</a>,
<a href="#argoproj.io/v1alpha1.NativeStrategy">NativeStrategy</a>)
</p>
<p>
<p>
PersistenceStrategy defines the strategy of persistence
</p>
</p>
<table>
<thead>
<tr>
<th>
Field
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>storageClassName</code></br> <em> string </em>
</td>
<td>
<em>(Optional)</em>
<p>
Name of the StorageClass required by the claim. More info:
<a href="https://kubernetes.io/docs/concepts/storage/persistent-volumes#class-1">https://kubernetes.io/docs/concepts/storage/persistent-volumes#class-1</a>
</p>
</td>
</tr>
<tr>
<td>
<code>accessMode</code></br> <em>
<a href="https://v1-18.docs.kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#persistentvolumeaccessmode-v1-core">
Kubernetes core/v1.PersistentVolumeAccessMode </a> </em>
</td>
<td>
<em>(Optional)</em>
<p>
Available access modes such as ReadWriteOnce, ReadWriteMany
<a href="https://kubernetes.io/docs/concepts/storage/persistent-volumes/#access-modes">https://kubernetes.io/docs/concepts/storage/persistent-volumes/#access-modes</a>
</p>
</td>
</tr>
<tr>
<td>
<code>volumeSize</code></br> <em>
k8s.io/apimachinery/pkg/api/resource.Quantity </em>
</td>
<td>
<p>
Volume size, e.g. 10Gi
</p>
</td>
</tr>
</tbody>
</table>
<hr/>
<p>
<em> Generated with <code>gen-crd-api-reference-docs</code>. </em>
</p>
