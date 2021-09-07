Redis is the only required prerequisite for all Tyk installations, used as a key store and for distributed rate limiting. In this tutorial we'll run through the use of our _simple-redis_ chart.  
**Caution:** this _simple-redis_ chart is designed for evaluation purposes only and is not for production use. You can find recommended charts and further details referenced in our documentation.  

*  Install Redis to the tyk namespace using the _simple-redis_ chart.  
`helm install redis tyk-helm/simple-redis -n tyk`{{execute}}

*  Check that the Redis pod is ready and in the **"Running"** status before moving to the next stage.  
`kubectl get pods -n tyk`{{execute}}
