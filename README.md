# Kubernetes_Learning

What K8s objects are essential for a 3-tier app?”, this is the money list:

$ kubectl api-resources | grep -Ei 'pods|service|deployment|Ingress|configmap|secret|PVC|PV|namespace|statefulset|HPA'
NAME                                SHORTNAMES   APIVERSION                        NAMESPACED   KIND
configmaps                          cm           v1                                true         ConfigMap
namespaces                          ns           v1                                false        Namespace
persistentvolumeclaims              pvc          v1                                true         PersistentVolumeClaim
persistentvolumes                   pv           v1                                false        PersistentVolume
pods                                po           v1                                true         Pod
secrets                                          v1                                true         Secret
serviceaccounts                     sa           v1                                true         ServiceAccount
services                            svc          v1                                true         Service
apiservices                                      apiregistration.k8s.io/v1         false        APIService
deployments                         deploy       apps/v1                           true         Deployment
statefulsets                        sts          apps/v1                           true         StatefulSet
horizontalpodautoscalers            hpa          autoscaling/v2                    true         HorizontalPodAutoscaler
ingressclasses                                   networking.k8s.io/v1              false        IngressClass
ingresses                           ing          networking.k8s.io/v1              true         Ingress
servicecidrs                                     networking.k8s.io/v1              false        ServiceCIDR
