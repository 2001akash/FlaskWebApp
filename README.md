1.**Approach**
Our approach involved a systematic setup, leveraging GitOps principles. We containerized the application, configured Argo CD for automated deployments, and employed Argo Rollouts for canary releases.

2. **Challenges and Solutions**
Challenge 1: Integration with Argo CD
Solution: Thoroughly followed the Argo CD documentation, ensuring correct installation and configuration on the Kubernetes cluster.
Challenge 2: Canary Release Fine-tuning
Solution: Experimented with Argo Rollouts parameters, iteratively adjusting the canary release strategy for optimal results.
3. **Cleanup Instructions**
To remove all resources created during this assignment from the Kubernetes cluster, follow these steps:

Run kubectl delete -f <path-to-manifests> to delete the deployed application and Argo CD configurations.
Use kubectl delete -f <argorollouts-manifest> to remove the Argo Rollouts resources.
Optionally, clean up Docker images from the container registry.

4.**Conclusion**
In conclusion, this assignment provided hands-on experience with GitOps practices, Argo CD, and Argo Rollouts. The implemented pipeline ensures automated, reliable, and controlled deployments of the web application in a Kubernetes environment.

